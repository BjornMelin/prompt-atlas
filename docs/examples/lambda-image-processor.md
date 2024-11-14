# Example: AWS Lambda Image Processing Service

This example demonstrates how to use our prompts to build a production-ready AWS Lambda function for image processing.

## Table of Contents

- [Project Overview](#project-overview)
- [Development Process](#development-process)
- [Implementation Details](#implementation-details)
- [Deployment and Testing](#deployment-and-testing)
- [Lessons Learned](#lessons-learned)

## Project Overview

### Business Requirements

- Process uploaded images for an e-commerce platform
- Create multiple sizes of each image
- Store metadata in DynamoDB
- Notify other services when processing is complete

### Technical Requirements

- Handle images up to 5MB
- Process within 10 seconds
- Support JPG and PNG formats
- Maintain original aspect ratios

## Development Process

### 1. Initial Prompt

```markdown
I need to develop an AWS Lambda function for image processing with:

1. Function Specifications:

   - Runtime: Python 3.11
   - Memory: 1024 MB
   - Timeout: 30 seconds
   - Concurrency: 100

2. Event Sources:

   - S3 bucket upload
   - Event pattern: _.jpg, _.png
   - DLQ for failed processing

3. Integration Points:
   - Input: S3 bucket
   - Output: Processed images to S3
   - Metadata: DynamoDB
   - Notifications: EventBridge

Current focus: Core image processing
```

### 2. Infrastructure as Code

```yaml
Resources:
  ProcessImageFunction:
    Type: AWS::Serverless::Function
    Properties:
      Handler: handler.process_image
      Runtime: python3.11
      MemorySize: 1024
      Timeout: 30
      Environment:
        Variables:
          OUTPUT_BUCKET: !Ref OutputBucket
          METADATA_TABLE: !Ref MetadataTable
      Events:
        ImageUpload:
          Type: S3
          Properties:
            Bucket: !Ref InputBucket
            Events: s3:ObjectCreated:*
```

## Implementation Details

### Core Processing Function

```python
import boto3
from PIL import Image
import os

def process_image(event, context):
    # Get image from S3
    s3_client = boto3.client('s3')
    bucket = event['Records'][0]['s3']['bucket']['name']
    key = event['Records'][0]['s3']['object']['key']

    # Download image
    download_path = f"/tmp/{key}"
    s3_client.download_file(bucket, key, download_path)

    # Process image
    sizes = [(800, 800), (400, 400), (200, 200)]
    output_paths = []

    for size in sizes:
        output_path = f"/tmp/resized_{size[0]}x{size[1]}_{key}"
        with Image.open(download_path) as img:
            img.thumbnail(size)
            img.save(output_path)
        output_paths.append(output_path)

    # Upload processed images
    for path in output_paths:
        upload_key = f"processed/{os.path.basename(path)}"
        s3_client.upload_file(path, os.environ['OUTPUT_BUCKET'], upload_key)

    return {
        'statusCode': 200,
        'body': f"Processed {len(output_paths)} versions of {key}"
    }
```

### Error Handling

```python
try:
    process_image(event, context)
except Exception as e:
    # Log error
    print(f"Error processing image: {str(e)}")

    # Send to DLQ
    sqs = boto3.client('sqs')
    sqs.send_message(
        QueueUrl=os.environ['DLQ_URL'],
        MessageBody=json.dumps({
            'error': str(e),
            'event': event
        })
    )

    raise e
```

## Deployment and Testing

### Deployment Process

1. Package Lambda function
2. Deploy SAM template
3. Configure triggers
4. Verify permissions

### Test Cases

1. Standard JPG/PNG files
2. Large files (near 5MB)
3. Invalid file types
4. Concurrent uploads
5. Error scenarios

## Lessons Learned

### 1. Performance Optimization

- Optimal memory configuration
- Cold start mitigation
- Efficient image processing

### 2. Error Handling

- Comprehensive error catching
- DLQ implementation
- Monitoring and alerts

### 3. Cost Optimization

- Memory vs performance
- Concurrent execution
- Storage management

## Monitoring and Metrics

### CloudWatch Metrics

- Execution duration
- Error rates
- Throttling
- Memory usage

### Custom Metrics

- Image processing time
- Output file sizes
- Success rates
- DLQ messages

## Future Improvements

1. **Performance**

   - Implement caching
   - Optimize algorithms
   - Reduce cold starts

2. **Features**

   - Additional formats
   - Custom sizes
   - Metadata extraction

3. **Operations**

   - Enhanced monitoring
   - Automated testing
   - Cost optimization

This example demonstrates:

- Proper prompt usage
- Implementation details
- Best practices
- Common patterns
- Learning opportunities

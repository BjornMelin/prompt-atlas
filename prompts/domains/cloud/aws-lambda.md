# AWS Lambda Function Development

## Description
This prompt template helps you design and implement AWS Lambda functions with best practices for various use cases, including data processing, API backends, and event-driven workflows.

## Use Cases
- Serverless API backends
- Data transformation and ETL processes
- Event-driven architectures
- Scheduled tasks and cron jobs
- Real-time file processing

## Parameters
- `[RUNTIME]`: Programming language runtime (Python, Node.js, Java, etc.)
- `[MEMORY]`: Memory allocation in MB (128MB to 10GB)
- `[TIMEOUT]`: Execution timeout in seconds (1-900s)
- `[EVENT_SOURCE]`: Trigger for the Lambda (S3, API Gateway, EventBridge, etc.)
- `[INTEGRATION_POINTS]`: External services the Lambda will interact with

## Example Usage

```markdown
I need to develop an AWS Lambda function for image processing with:

1. Function Specifications:
   - Runtime: [RUNTIME] (e.g., Python 3.11)
   - Memory: [MEMORY] (e.g., 1024 MB)
   - Timeout: [TIMEOUT] (e.g., 30 seconds)
   - Concurrency limits: [CONCURRENCY] (e.g., 100)

2. Event Sources:
   - Trigger type: [EVENT_SOURCE] (e.g., S3 bucket upload)
   - Event pattern: [PATTERN] (e.g., *.jpg, *.png)
   - Error handling: [ERROR_STRATEGY] (e.g., DLQ for failed processing)

3. Integration Points:
   - [INTEGRATION_POINTS] (e.g., S3 for storage, DynamoDB for metadata)
   - Authentication requirements: [AUTH_REQUIREMENTS]
   - Network configuration: [NETWORK_CONFIG] (e.g., VPC requirements)

4. Development Workflow:
   - Testing approach: [TESTING_STRATEGY]
   - Deployment method: [DEPLOYMENT_METHOD] (e.g., SAM, Serverless Framework)
   - CI/CD integration: [CICD_PIPELINE]

Focus area: [SPECIFIC_FUNCTIONALITY] (e.g., image resize operation)
```

## Expected Output
The AI assistant should provide a comprehensive solution including:

1. Lambda function code implementing the requested functionality
2. Infrastructure as Code (IaC) for deployment (e.g., SAM template, Serverless Framework)
3. IAM permissions and policies 
4. Error handling and logging implementation
5. Testing approach and examples
6. Deployment instructions

## Customization Guide
- For simpler functions, you can omit concurrency limits and CI/CD integration
- Add specific performance requirements if critical
- Include specific AWS region if required
- For VPC-connected Lambdas, specify subnet and security group requirements
- For third-party integrations, specify authentication and endpoint details

## Version
- Current Version: 1.0
- Last Updated: 2025-05-07

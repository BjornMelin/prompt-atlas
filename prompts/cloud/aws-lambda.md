# AWS Lambda Development Prompts

## Table of Contents

- [Function Development](#function-development)
- [Event Processing](#event-processing-function)
- [Integration Patterns](#integration-patterns)
- [Optimization](#optimization)
- [Examples](#examples)

## Function Development

### Basic Lambda Function

```markdown
I need to develop an AWS Lambda function for [use case] with:

1. Function Specifications:

   - Runtime: [Python/Node.js/Java/etc]
   - Memory allocation: [MB]
   - Timeout settings: [seconds]
   - Concurrency limits: [number]
   - VPC requirements: [Yes/No]

2. Event Sources:

   - Trigger type: [API Gateway/S3/EventBridge/etc]
   - Event schema
   - Event filtering patterns
   - Dead letter queue strategy

3. Integration Requirements:

   - AWS Services: [list required services]
   - External APIs
   - Database connections
   - Shared resources

4. Development Workflow:
   - Local testing approach
   - CI/CD integration
   - Deployment strategy
   - Version management

Focus area: [specific functionality]
```

### Event Processing Function

```markdown
I need to develop an event processing Lambda with:

1. Event Specifications:

   - Source service: [SQS/SNS/EventBridge/etc]
   - Message format: [JSON/XML/Binary]
   - Processing requirements
   - Error handling strategy

2. Performance Requirements:

   - Batch size: [number of events]
   - Processing time limits
   - Concurrent executions
   - Resource constraints

3. Resilience Patterns:
   - Retry strategy
   - DLQ configuration
   - Circuit breaker patterns
   - Fallback mechanisms

Current focus: [specific processing step]
```

## Integration Patterns

### API Integration

```markdown
I need to integrate Lambda with API Gateway:

1. API Specifications:

   - HTTP methods: [GET/POST/etc]
   - Authorization: [IAM/Cognito/Custom]
   - Request/Response models
   - CORS configuration

2. Integration Type:

   - Proxy integration
   - Custom integration
   - VPC link requirements
   - Direct integrations

3. Security Requirements:
   - Authentication method
   - Authorization scopes
   - API key usage
   - WAF integration
```

### Database Integration

```markdown
I need to integrate Lambda with [database]:

1. Connection Requirements:

   - Connection pooling
   - Credential management
   - VPC configuration
   - Timeout handling

2. Query Patterns:

   - CRUD operations
   - Batch processing
   - Transaction management
   - Error handling

3. Performance Optimization:
   - Connection reuse
   - Query optimization
   - Cache strategy
   - Resource management
```

## Optimization

### Performance Optimization

```markdown
Help me optimize Lambda function [name] for:

1. Current Metrics:

   - Average duration: [ms]
   - Memory usage: [MB]
   - Cold start frequency
   - Error rate: [%]

2. Target Improvements:

   - Response time goals
   - Memory utilization
   - Cost reduction
   - Reliability targets

3. Optimization Areas:
   - Code efficiency
   - Memory allocation
   - Dependency management
   - Connection handling
```

## Examples

### REST API Lambda

```markdown
I need to develop a REST API Lambda for user management:

1. Function Specifications:

   - Runtime: Node.js 18
   - Memory: 512 MB
   - Timeout: 10 seconds
   - Concurrency: 50

2. API Endpoints:

   - GET /users
   - POST /users
   - PUT /users/{id}
   - DELETE /users/{id}

3. Integration Points:
   - DynamoDB for user data
   - Cognito for authentication
   - SES for notifications
   - S3 for user uploads

Focus: User creation endpoint
```

### Event Processing Example

```markdown
I need an event processing Lambda for order processing:

1. Event Source:

   - SQS FIFO queue
   - Order events in JSON
   - 100 messages per batch
   - 5-minute timeout

2. Processing Steps:

   - Validate order data
   - Update inventory
   - Process payment
   - Send confirmation

3. Integration Points:
   - DynamoDB for orders
   - Payment gateway API
   - SNS for notifications
   - EventBridge for workflow

Focus: Payment processing step
```

## Best Practices

1. **Function Design**

   - Single responsibility
   - Stateless operation
   - Idempotent processing
   - Proper error handling

2. **Performance**

   - Optimize memory
   - Manage cold starts
   - Connection pooling
   - Efficient logging

3. **Security**

   - Least privilege IAM
   - Secret management
   - Input validation
   - Output sanitization

4. **Monitoring**

   - CloudWatch metrics
   - Custom metrics
   - Tracing with X-Ray
   - Log aggregation

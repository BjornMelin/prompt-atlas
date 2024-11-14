# Serverless Architecture Development Prompts

## Table of Contents
- [Application Architecture](#application-architecture)
- [Service Integration](#service-integration)
- [State Management](#state-management)
- [Deployment Patterns](#deployment-patterns)
- [Examples](#examples)

## Application Architecture

### Microservices Architecture
```markdown
I need to design a serverless microservices architecture for [use case] with:
1. Service Boundaries:
   - Domain definitions
   - Service responsibilities
   - Integration points
   - Data ownership

2. Technical Stack:
   - Compute services: [Lambda/Fargate/etc]
   - API management: [API Gateway/AppSync]
   - Data storage: [DynamoDB/Aurora/etc]
   - Message queues: [SQS/EventBridge/etc]

3. Cross-cutting Concerns:
   - Authentication/Authorization
   - Monitoring strategy
   - Error handling
   - Data consistency

Current focus: [specific service/component]
```

### Event-Driven Architecture
```markdown
I need to design an event-driven serverless system with:
1. Event Flow:
   - Event sources
   - Event types
   - Processing patterns
   - State transitions

2. Technical Components:
   - Event bus: [EventBridge/SNS/etc]
   - Processing services
   - Storage solutions
   - Integration points

3. Operational Requirements:
   - Event ordering
   - Duplicate handling
   - Error recovery
   - Monitoring needs
```

## Service Integration

### API Design
```markdown
Help me design a serverless API with:
1. API Specifications:
   - REST/GraphQL design
   - Authentication method
   - Rate limiting
   - CORS requirements

2. Implementation:
   - Lambda integration
   - Custom authorizers
   - Request/Response mapping
   - Error handling

3. Management:
   - API versioning
   - Documentation
   - Monitoring
   - Usage plans
```

### Data Flow
```markdown
I need to design data flow for serverless application:
1. Data Sources:
   - Input methods
   - Data formats
   - Volume expectations
   - Frequency patterns

2. Processing Requirements:
   - Transformation needs
   - Validation rules
   - Business logic
   - Error handling

3. Storage Solutions:
   - Primary storage
   - Caching strategy
   - Backup approach
   - Retention policy
```

## State Management

### Database Design
```markdown
Help me design a serverless database architecture:
1. Requirements:
   - Data model
   - Access patterns
   - Scaling needs
   - Consistency requirements

2. Technical Decisions:
   - Database type: [DynamoDB/Aurora/etc]
   - Table design
   - Index strategy
   - Backup strategy

3. Implementation:
   - Connection handling
   - Query patterns
   - Transaction support
   - Error handling
```

## Deployment Patterns

### Infrastructure as Code
```markdown
I need to create IaC for serverless application:
1. Resource Definitions:
   - Compute resources
   - Storage resources
   - Network setup
   - Security config

2. Environment Strategy:
   - Stage definitions
   - Variable management
   - Service dependencies
   - Resource policies

3. Deployment Process:
   - CI/CD integration
   - Testing strategy
   - Rollback plan
   - Monitoring setup
```

## Examples

### E-commerce Platform
```markdown
I need to design a serverless e-commerce platform:
1. Components:
   - Product catalog service
   - Order processing system
   - Payment integration
   - User management

2. Technical Stack:
   - API Gateway + Lambda
   - DynamoDB for products/orders
   - EventBridge for workflows
   - S3 for static content

3. Integration Points:
   - Payment gateway
   - Shipping service
   - Email service
   - Analytics platform

Focus: Order processing workflow
```

### Real-time Analytics
```markdown
Design a serverless real-time analytics system:
1. Requirements:
   - Event ingestion
   - Real-time processing
   - Data aggregation
   - Visualization

2. Architecture:
   - Kinesis Data Streams
   - Lambda processors
   - DynamoDB for storage
   - API Gateway for queries

3. Operational Needs:
   - Scaling strategy
   - Error handling
   - Data retention
   - Cost optimization

Focus: Real-time data processing
```

## Best Practices

1. **Architecture Design**
   - Loose coupling
   - High cohesion
   - Event-driven patterns
   - Stateless services

2. **Data Management**
   - Data consistency
   - Access patterns
   - Backup strategy
   - Security controls

3. **Operational Excellence**
   - Monitoring setup
   - Logging strategy
   - Alert configuration
   - Cost management

4. **Security**
   - Authentication
   - Authorization
   - Encryption
   - Compliance

# Microservices Architecture Prompts

## Table of Contents
- [Architecture Design](#architecture-design)
- [Service Design](#service-design)
- [Integration Patterns](#integration-patterns)
- [Deployment Strategies](#deployment-strategies)
- [Examples](#examples)

## Architecture Design

### System Architecture
```markdown
Design microservices architecture for [use case] with:
1. Domain Design:
   - Service boundaries
   - Data ownership
   - Communication patterns
   - Shared resources

2. Technical Stack:
   - Service technology: [Node/Java/Go/etc]
   - Database choices
   - Message broker
   - API gateway

3. Cross-cutting Concerns:
   - Authentication/Authorization
   - Logging/Monitoring
   - Error handling
   - Data consistency

4. Infrastructure Requirements:
   - Container orchestration
   - Service discovery
   - Load balancing
   - Configuration management

Current focus: [specific service/component]
```

### Service Decomposition
```markdown
Help decompose monolith into microservices:
1. Current State:
   - Application overview
   - Component coupling
   - Data dependencies
   - Integration points

2. Decomposition Strategy:
   - Service boundaries
   - Migration phases
   - Data splitting
   - Interface design

3. Implementation Plan:
   - Priority order
   - Technical approach
   - Risk mitigation
   - Success criteria
```

## Service Design

### Individual Service
```markdown
Design microservice for [functionality] with:
1. Service Specifications:
   - Core functionality
   - API design
   - Data model
   - External dependencies

2. Technical Requirements:
   - Performance targets
   - Scalability needs
   - Reliability goals
   - Resource limits

3. Integration Points:
   - Synchronous APIs
   - Event publishing
   - Data consistency
   - Error handling

4. Operational Needs:
   - Monitoring strategy
   - Logging approach
   - Health checks
   - Deployment process
```

## Integration Patterns

### Service Communication
```markdown
Design service communication patterns for:
1. Synchronous Communication:
   - REST APIs
   - gRPC services
   - GraphQL endpoints
   - Circuit breakers

2. Asynchronous Messaging:
   - Event format
   - Message broker
   - Dead letter queues
   - Retry policies

3. Data Consistency:
   - Saga pattern
   - Event sourcing
   - CQRS approach
   - Compensation logic
```

### API Gateway
```markdown
Design API gateway layer with:
1. Gateway Requirements:
   - Route management
   - Authentication
   - Rate limiting
   - Request transformation

2. Implementation:
   - Gateway technology
   - Routing rules
   - Security controls
   - Monitoring setup

3. Cross-cutting Features:
   - Request logging
   - Error handling
   - Response caching
   - Circuit breaking
```

## Deployment Strategies

### Deployment Design
```markdown
Create deployment strategy for microservices:
1. Infrastructure:
   - Container platform: [K8s/ECS/etc]
   - Service mesh
   - Monitoring tools
   - Log aggregation

2. Deployment Process:
   - CI/CD pipeline
   - Blue-green deployment
   - Canary releases
   - Rollback strategy

3. Configuration Management:
   - Config storage
   - Secret management
   - Environment handling
   - Version control
```

## Examples

### E-commerce Platform
```markdown
Design microservices for e-commerce:
1. Services:
   - Product service
   - Order service
   - User service
   - Payment service
   - Inventory service

2. Integration:
   - API Gateway
   - Event bus
   - Service mesh
   - Data consistency

3. Technical Stack:
   - Node.js services
   - MongoDB/PostgreSQL
   - RabbitMQ
   - Redis cache

Focus: Order processing flow
```

### Payment Processing
```markdown
Design payment processing microservices:
1. Components:
   - Payment service
   - Fraud detection
   - Transaction history
   - Notification service

2. Requirements:
   - High availability
   - Data consistency
   - Audit logging
   - Security controls

3. Implementation:
   - Saga pattern
   - Event sourcing
   - CQRS
   - Idempotency

Focus: Transaction consistency
```

## Best Practices

1. **Service Design**
   - Single responsibility
   - Loose coupling
   - High cohesion
   - Independent deployment

2. **Data Management**
   - Data ownership
   - Eventual consistency
   - ACID boundaries
   - Event-driven updates

3. **Resilience**
   - Circuit breakers
   - Retry policies
   - Fallback mechanisms
   - Graceful degradation

4. **Observability**
   - Distributed tracing
   - Centralized logging
   - Metrics collection
   - Health monitoring

5. **Security**
   - Service authentication
   - Authorization
   - Secret management
   - Network security

6. **DevOps**
   - Automated deployment
   - Configuration management
   - Container orchestration
   - Service discovery

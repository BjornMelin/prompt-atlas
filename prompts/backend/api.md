# API Development Prompts

## Table of Contents
- [REST API Design](#rest-api-design)
- [GraphQL API Design](#graphql-api-design)
- [API Security](#api-security)
- [Performance Optimization](#performance-optimization)
- [Examples](#examples)

## REST API Design

### Basic REST API
```markdown
I need to design a REST API for [use case] with:
1. API Specifications:
   - Resource definitions
   - HTTP methods
   - Response formats
   - Status codes

2. Endpoint Design:
   - URL structure
   - Query parameters
   - Request bodies
   - Response schemas

3. Technical Requirements:
   - Authentication method
   - Rate limiting
   - Caching strategy
   - CORS policy

4. Documentation:
   - OpenAPI/Swagger spec
   - API reference
   - Integration guides
   - Examples

Current focus: [specific endpoint/resource]
```

### API Versioning
```markdown
Help design API versioning strategy with:
1. Version Requirements:
   - Versioning method: [URL/Header/Parameter]
   - Backward compatibility
   - Deprecation policy
   - Migration path

2. Technical Implementation:
   - Version routing
   - Request handling
   - Response formatting
   - Documentation approach

3. Operational Concerns:
   - Version lifecycle
   - Support timeline
   - Client communication
   - Monitoring strategy
```

## GraphQL API Design

### GraphQL Schema
```markdown
Design a GraphQL API for [use case] with:
1. Schema Design:
   - Type definitions
   - Query operations
   - Mutation operations
   - Subscription needs

2. Resolver Implementation:
   - Data sources
   - Authentication
   - Error handling
   - Performance optimization

3. Technical Requirements:
   - Batching strategy
   - Caching approach
   - Real-time updates
   - File handling

4. Client Support:
   - Query complexity
   - Rate limiting
   - Persisted queries
   - Documentation
```

## API Security

### Security Implementation
```markdown
Implement API security for [service] with:
1. Authentication:
   - Auth method: [JWT/OAuth/API Key]
   - Token management
   - Session handling
   - Refresh strategy

2. Authorization:
   - Role definitions
   - Permission model
   - Access control
   - Resource policies

3. Security Controls:
   - Input validation
   - Rate limiting
   - Request signing
   - Audit logging

4. Compliance:
   - Data protection
   - Privacy controls
   - Regulatory requirements
   - Security headers
```

## Performance Optimization

### API Optimization
```markdown
Optimize API performance for:
1. Current Metrics:
   - Response times
   - Request volume
   - Error rates
   - Resource usage

2. Optimization Areas:
   - Query efficiency
   - Caching strategy
   - Connection pooling
   - Response compression

3. Scaling Strategy:
   - Load balancing
   - Auto-scaling
   - Database optimization
   - Cache distribution

4. Monitoring:
   - Performance metrics
   - Error tracking
   - Usage analytics
   - Alerts setup
```

## Examples

### E-commerce API
```markdown
Design REST API for e-commerce platform:
1. Resources:
   - /products
     - GET /products
     - GET /products/{id}
     - POST /products
     - PUT /products/{id}
     - DELETE /products/{id}
   - /orders
   - /users
   - /cart

2. Features:
   - Product search/filter
   - Order processing
   - Cart management
   - User profiles

3. Technical Stack:
   - Node.js/Express
   - PostgreSQL
   - Redis caching
   - JWT auth

Focus: Product search optimization
```

### Analytics API
```markdown
Design analytics data API with:
1. Requirements:
   - Real-time metrics
   - Historical data
   - Aggregations
   - Export capabilities

2. Implementation:
   - GraphQL schema
   - Time-series data
   - Caching strategy
   - Rate limiting

3. Performance:
   - Query optimization
   - Response pagination
   - Data denormalization
   - Background processing

Focus: Real-time metrics delivery
```

## Best Practices

1. **API Design**
   - Clear naming conventions
   - Consistent patterns
   - Proper HTTP methods
   - Meaningful status codes

2. **Security**
   - Strong authentication
   - Proper authorization
   - Input validation
   - Rate limiting

3. **Performance**
   - Efficient queries
   - Proper caching
   - Response optimization
   - Resource management

4. **Documentation**
   - Clear specifications
   - Usage examples
   - Error descriptions
   - Integration guides

5. **Monitoring**
   - Performance metrics
   - Error tracking
   - Usage analytics
   - Health checks

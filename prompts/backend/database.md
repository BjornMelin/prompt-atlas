# Database Design and Optimization Prompts

## Table of Contents

- [Database Design](#database-design)
- [Query Optimization](#query-optimization)
- [Data Migration](#data-migration)
- [Performance Tuning](#performance-tuning)
- [Examples](#examples)

## Database Design

### Schema Design

```markdown
I need to design a database schema for [use case] with:

1. Requirements:

   - Data model
   - Relationships
   - Constraints
   - Indexing strategy

2. Access Patterns:

   - Read operations
   - Write operations
   - Query patterns
   - Search requirements

3. Technical Considerations:

   - Database type: [SQL/NoSQL]
   - Scaling strategy
   - Backup approach
   - Replication needs

4. Performance Requirements:
   - Query response times
   - Write throughput
   - Concurrency handling
   - Data volume projections
```

### NoSQL Design

```markdown
Design NoSQL database for [use case] with:

1. Data Structure:

   - Document design
   - Key patterns
   - Denormalization strategy
   - Secondary indexes

2. Access Requirements:

   - Query patterns
   - Update patterns
   - Consistency needs
   - Partition strategy

3. Technical Specs:
   - Database choice: [DynamoDB/MongoDB/etc]
   - Throughput requirements
   - Storage estimates
   - Scaling approach
```

## Query Optimization

### Performance Tuning

```markdown
Optimize database queries for:

1. Current State:

   - Slow queries
   - Resource usage
   - Pain points
   - Growth projections

2. Optimization Areas:

   - Index usage
   - Query structure
   - Data organization
   - Caching strategy

3. Implementation:

   - Index changes
   - Query rewrites
   - Schema updates
   - Configuration tuning

4. Monitoring:
   - Performance metrics
   - Resource utilization
   - Query analysis
   - Alert setup
```

## Data Migration

### Migration Strategy

```markdown
Plan database migration from [source] to [target] with:

1. Migration Requirements:

   - Data volume
   - Downtime constraints
   - Validation needs
   - Rollback strategy

2. Technical Approach:

   - Migration method
   - Tools selection
   - Testing strategy
   - Verification process

3. Risk Management:

   - Data integrity
   - Performance impact
   - Security concerns
   - Compliance requirements

4. Implementation Plan:
   - Timeline
   - Resource needs
   - Communication plan
   - Success criteria
```

## Performance Tuning

### Database Optimization

```markdown
Optimize database performance for:

1. Current Issues:

   - Slow queries: [list]
   - Resource bottlenecks
   - Scaling limitations
   - Operational challenges

2. Optimization Goals:

   - Response time targets
   - Throughput requirements
   - Resource utilization
   - Cost constraints

3. Implementation Strategy:

   - Schema optimization
   - Query tuning
   - Index management
   - Configuration updates

4. Monitoring Setup:
   - Performance metrics
   - Resource tracking
   - Query analysis
   - Alert configuration
```

## Examples

### E-commerce Database

```markdown
Design database for e-commerce platform:

1. Schema Requirements:

   - Products
   - Orders
   - Customers
   - Inventory
   - Reviews

2. Access Patterns:

   - Product search/filter
   - Order processing
   - Inventory updates
   - Analytics queries

3. Technical Stack:
   - PostgreSQL
   - Redis cache
   - Read replicas
   - Backup strategy

Focus: Order processing optimization
```

### Real-time Analytics

```markdown
Design analytics database with:

1. Requirements:

   - Time-series data
   - Real-time updates
   - Historical queries
   - Aggregations

2. Implementation:

   - TimescaleDB
   - Materialized views
   - Partitioning strategy
   - Retention policy

3. Performance:
   - Write optimization
   - Query efficiency
   - Data compression
   - Cache strategy

Focus: Real-time ingestion
```

## Best Practices

1. **Schema Design**

   - Proper normalization
   - Clear naming
   - Appropriate types
   - Necessary constraints

2. **Indexing Strategy**

   - Selective indexes
   - Covering indexes
   - Index maintenance
   - Impact analysis

3. **Query Optimization**

   - Efficient queries
   - Proper joins
   - Index usage
   - Query planning

4. **Performance**

   - Resource monitoring
   - Query analysis
   - Configuration tuning
   - Capacity planning

5. **Operational Excellence**

   - Backup strategy
   - Monitoring setup
   - Maintenance plans
   - Documentation

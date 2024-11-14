# Cloud Architecture Design Prompts

## Table of Contents
- [System Architecture](#system-architecture)
- [Migration Planning](#migration-planning)
- [Infrastructure Design](#infrastructure-design)
- [Security Architecture](#security-architecture)
- [Cost Optimization](#cost-optimization)
- [Examples](#examples)

## System Architecture

### Well-Architected System Design
```markdown
I need to design a cloud architecture following Well-Architected principles for [use case] with:
1. System Requirements:
   - Availability target: [99.9%/99.99%/etc]
   - Performance requirements: [latency/throughput]
   - Scalability needs: [users/requests/data volume]
   - Budget constraints: [monthly/annual cost]

2. Technical Components:
   - Compute strategy: [EC2/ECS/Lambda/etc]
   - Storage solutions: [S3/EFS/EBS/etc]
   - Database choices: [RDS/DynamoDB/etc]
   - Caching approach: [ElastiCache/DAX/etc]

3. Architectural Decisions:
   - High availability strategy
   - Disaster recovery plan
   - Data backup approach
   - Monitoring solution

4. Security Requirements:
   - Compliance needs: [SOC2/HIPAA/etc]
   - Network design: [VPC/subnets/NACLs]
   - Identity management: [IAM/SSO/etc]
   - Data protection: [encryption/masking]

Current focus: [specific component/requirement]
```

## Migration Planning

### Cloud Migration Strategy
```markdown
Help me plan migration from [current state] to AWS with:
1. Current Environment:
   - Infrastructure inventory
   - Application dependencies
   - Data volumes
   - Integration points

2. Migration Strategy:
   - Approach: [Rehost/Replatform/Refactor]
   - Phasing plan
   - Timeline
   - Success criteria

3. Technical Requirements:
   - Network connectivity
   - Data transfer method
   - Security controls
   - Compliance requirements

4. Operational Considerations:
   - Monitoring strategy
   - Backup procedures
   - Support model
   - Training needs
```

## Infrastructure Design

### Network Architecture
```markdown
Design a cloud network architecture with:
1. Network Requirements:
   - Connectivity needs: [VPN/Direct Connect/Internet]
   - Segmentation strategy
   - IP addressing plan
   - DNS strategy

2. Security Controls:
   - Access controls
   - Firewall rules
   - WAF configuration
   - DDoS protection

3. Performance Requirements:
   - Latency targets
   - Bandwidth needs
   - Regional distribution
   - Failover strategy

4. Operational Requirements:
   - Monitoring approach
   - Logging strategy
   - Alerting needs
   - Automation requirements
```

### Multi-Region Design
```markdown
Help design multi-region architecture for:
1. Regional Strategy:
   - Primary region: [region]
   - Secondary regions: [regions]
   - Failover approach
   - Data replication

2. Service Distribution:
   - Regional services
   - Global services
   - Edge locations
   - Route 53 strategy

3. Consistency Requirements:
   - Data synchronization
   - State management
   - Cache invalidation
   - Conflict resolution

4. Operational Approach:
   - Deployment strategy
   - Monitoring setup
   - Incident response
   - Cost management
```

## Security Architecture

### Security Design
```markdown
Design security architecture for [system] with:
1. Security Requirements:
   - Compliance frameworks
   - Data classification
   - Access controls
   - Audit requirements

2. Technical Controls:
   - Identity management
   - Network security
   - Data protection
   - Key management

3. Operational Security:
   - Monitoring strategy
   - Incident response
   - Patch management
   - Vulnerability scanning

4. Documentation Needs:
   - Security policies
   - Procedures
   - Compliance evidence
   - Architecture diagrams
```

## Cost Optimization

### Cost-Optimized Architecture
```markdown
Help optimize cloud architecture costs for:
1. Current State:
   - Monthly spend: [$amount]
   - Resource utilization
   - Service breakdown
   - Growth projections

2. Optimization Targets:
   - Cost reduction goals
   - Performance requirements
   - Reliability needs
   - Operational overhead

3. Strategy:
   - Reserved capacity
   - Spot usage
   - Storage tiering
   - Service selection

4. Implementation:
   - Phase approach
   - Monitoring needs
   - Automation opportunities
   - Governance controls
```

## Examples

### E-commerce Platform
```markdown
Design cloud architecture for e-commerce platform:
1. Requirements:
   - 100K daily active users
   - 99.99% availability
   - Sub-second response time
   - PCI compliance

2. Components:
   - ECS for microservices
   - Aurora for transactions
   - ElastiCache for sessions
   - S3 for static content
   - CloudFront for CDN

3. Architecture:
   - Multi-AZ deployment
   - Auto-scaling groups
   - Load balancers
   - VPC design

Focus: Payment processing system
```

### Data Analytics Platform
```markdown
Design analytics platform architecture:
1. Requirements:
   - 5TB daily data ingestion
   - Real-time processing
   - Historical analysis
   - Data governance

2. Components:
   - Kinesis for streaming
   - EMR for processing
   - Redshift for warehouse
   - QuickSight for visualization

3. Data Flow:
   - Ingestion pipeline
   - Processing workflow
   - Storage strategy
   - Access patterns

Focus: Real-time analytics pipeline
```

## Best Practices

1. **Reliability**
   - Multi-AZ deployment
   - Auto-scaling
   - Fault tolerance
   - Disaster recovery

2. **Performance**
   - Caching strategy
   - Connection pooling
   - Load balancing
   - Content delivery

3. **Security**
   - Defense in depth
   - Least privilege
   - Encryption
   - Monitoring

4. **Cost**
   - Right-sizing
   - Reserved instances
   - Storage lifecycle
   - Resource cleanup

5. **Operational Excellence**
   - Infrastructure as Code
   - Automated deployment
   - Monitoring and logging
   - Documentation

Remember to:
- Start with business requirements
- Consider future growth
- Document decisions
- Review regularly

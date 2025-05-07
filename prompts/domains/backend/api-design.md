# API Design and Implementation

## Description
This prompt helps you design and implement robust, well-structured APIs using REST or GraphQL patterns, with proper error handling, authentication, and documentation.

## Use Cases
- Designing new API endpoints
- Creating API specifications (OpenAPI, GraphQL schema)
- Implementing RESTful services
- Building GraphQL resolvers and types
- Designing API authentication and authorization
- Creating API documentation

## Parameters
- `[API_TYPE]`: API architecture (REST, GraphQL, gRPC, etc.)
- `[BACKEND_LANGUAGE]`: Implementation language (Node.js, Python, Java, etc.)
- `[AUTH_METHOD]`: Authentication method (JWT, OAuth, API Key, etc.)
- `[PERFORMANCE_REQS]`: Performance requirements (response time, throughput)
- `[DATA_FORMAT]`: Response format (JSON, XML, Protocol Buffers, etc.)

## Example Usage

```markdown
I need to design a [API_TYPE] API for [USE_CASE] with:

1. API Specifications:
   - Endpoint requirements: [ENDPOINTS] (e.g., user management, content retrieval)
   - Data model: [DATA_MODEL] (e.g., user schema, content schema)
   - Response format: [DATA_FORMAT] (e.g., JSON)
   - Status codes and error handling: [ERROR_HANDLING] (e.g., standardized error responses)

2. Technical Requirements:
   - Backend language/framework: [BACKEND_LANGUAGE] (e.g., Node.js/Express)
   - Database interaction: [DATABASE] (e.g., MongoDB with Mongoose)
   - Authentication method: [AUTH_METHOD] (e.g., JWT)
   - Rate limiting: [RATE_LIMITS] (e.g., 100 requests per minute)

3. Security Requirements:
   - Authorization model: [AUTH_MODEL] (e.g., role-based access control)
   - Data validation: [VALIDATION] (e.g., input sanitization, schema validation)
   - Security headers: [SECURITY_HEADERS] (e.g., CORS policy, CSP)
   - Sensitive data handling: [DATA_SECURITY] (e.g., PII protection)

4. Documentation Requirements:
   - API specs format: [SPEC_FORMAT] (e.g., OpenAPI 3.0)
   - Documentation level: [DOC_LEVEL] (e.g., complete with examples)
   - Client examples: [CLIENT_EXAMPLES] (e.g., curl, JavaScript fetch)
   
Focus area: [SPECIFIC_FUNCTIONALITY] (e.g., implementing pagination for list endpoints)
```

## Expected Output
The AI assistant should provide:

1. API design with endpoints, methods, and data structures
2. Implementation code for the requested endpoints
3. Authentication and authorization implementation
4. Input validation and error handling
5. Documentation in the requested format
6. Testing approach and examples
7. Performance considerations

## Customization Guide
- For small APIs, you can simplify by focusing only on endpoints and data models
- For public APIs, emphasize documentation and developer experience
- For internal APIs, focus on integration patterns with other services
- Add specific performance requirements if the API handles high traffic
- Specify compliance requirements (GDPR, HIPAA, etc.) for regulated data
- For versioning, include your versioning strategy (URL path, header, etc.)

## Version
- Current Version: 1.0
- Last Updated: 2025-05-07

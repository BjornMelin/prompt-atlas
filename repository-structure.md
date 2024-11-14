# Repository Structure

```
ai-powered-development-prompts/
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   ├── bug_report.md               # Template for bug reports
│   │   ├── feature_request.md          # Template for feature requests
│   │   └── prompt_template.md          # Template for new prompt submissions
│   └── workflows/
│       ├── markdown-lint.yml           # GitHub Action for markdown linting
│       └── mlc_config.json             # Configuration for markdown link checker
│
├── docs/
│   ├── best-practices.md               # Development prompt best practices
│   ├── getting-started.md             # Quick start guide for new users
│   └── examples/
│       └── lambda-image-processor.md   # Example implementation
│
├── prompts/
│   ├── cloud/
│   │   ├── aws-lambda.md              # AWS Lambda development prompts
│   │   ├── serverless.md              # Serverless architecture prompts
│   │   └── architecture.md            # Cloud architecture design prompts
│   │
│   ├── frontend/
│   │   ├── react.md                   # React development prompts
│   │   ├── performance.md             # Frontend performance optimization
│   │   └── components.md              # Component design patterns
│   │
│   ├── backend/
│   │   ├── api.md                     # API development prompts
│   │   ├── database.md                # Database design prompts
│   │   └── microservices.md           # Microservices architecture prompts
│   │
│   └── mobile/
│       ├── react-native.md            # React Native development
│       ├── flutter.md                 # Flutter development
│       └── native.md                  # Native mobile development
│
├── CONTRIBUTING.md                     # Contribution guidelines
├── LICENSE                            # MIT License
└── README.md                          # Project documentation and overview
```

## Key Files and Their Contents:

1. **README.md**
   - Project overview
   - AWS certification badges
   - Features and capabilities
   - Quick start guide
   - Author information
   - Contribution links

2. **CONTRIBUTING.md**
   - Contribution guidelines
   - PR process
   - Style guide
   - Code of conduct
   - Review process

3. **.github/workflows/markdown-lint.yml**
   ```yaml
   name: Markdown Lint
   on:
     push:
       paths:
         - '**.md'
     # ... rest of workflow configuration
   ```

4. **docs/best-practices.md**
   - Prompt writing guidelines
   - Template usage
   - Common patterns
   - Success strategies

5. **prompts/cloud/aws-lambda.md**
   ```markdown
   # AWS Lambda Development Prompts
   
   ## Function Development Template
   ```markdown
   I need to develop an AWS Lambda function for [use case] with:
   1. Function Specifications:
      - Runtime: [Python/Node.js/Java/etc]
      # ... rest of template
   ```
   
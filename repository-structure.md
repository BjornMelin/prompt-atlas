# Repository Structure

```plaintext
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
│   ├── getting-started.md              # Quick start guide for new users
│   └── examples/
│       └── lambda-image-processor.md   # Example implementation
│
├── prompts/
│   ├── cloud/
│   │   ├── aws-lambda.md               # AWS Lambda development prompts
│   │   ├── serverless.md               # Serverless architecture prompts
│   │   └── architecture.md             # Cloud architecture design prompts
│   │
│   ├── frontend/
│   │   ├── react.md                    # React development prompts
│   │   ├── performance.md              # Frontend performance optimization
│   │   └── components.md               # Component design patterns
│   │
│   ├── backend/
│   │   ├── api.md                      # API development prompts
│   │   ├── database.md                 # Database design prompts
│   │   └── microservices.md            # Microservices architecture prompts
│   │
│   ├── mobile/
│   │   ├── react-native.md             # React Native development
│   │   ├── flutter.md                  # Flutter development
│   │   └── native.md                   # Native mobile development
│   │
│   ├── python/                         # Python-specific prompts
│   ├── typescript/                     # TypeScript-specific prompts
│   ├── prompt-engineering/             # Prompt engineering guides
│   └── cicd/                           # CI/CD pipeline templates
│
├── rules/
│   ├── cursor-ai-agent/                # Autonomous Cursor AI agent framework
│   │   ├── README.md                   # Overview and instructions
│   │   ├── system_prompt.md            # System prompt for Cursor AI
│   │   ├── project_config.md           # Long-term memory template
│   │   └── workflow_state.md           # Short-term memory and rules template
│   │
│   ├── cursorrules/                    # Rules for Cursor AI coding assistant
│   │   └── git_feature_workflow.mdc    # Git feature branch workflow rules
│   │
│   └── copilot/                        # GitHub Copilot optimization
│
├── CONTRIBUTING.md                     # Contribution guidelines
├── LICENSE                             # MIT License
├── README.md                           # Project documentation and overview
└── repository-structure.md             # Repository structure guide
```

## Key Files and Their Contents

1. **README.md**

   - Project overview
   - AWS certification badges
   - Features and capabilities
   - Quick start guide
   - Template categories
   - Author information
   - Contribution links
   - Citation information

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
         - "**.md"
     # ... rest of workflow configuration
   ```

4. **docs/best-practices.md**

   - Prompt writing guidelines
   - Template usage
   - Common patterns
   - Success strategies

5. **prompts/cloud/aws-lambda.md**

   ````markdown
   # AWS Lambda Development Prompts

   ## Function Development Template

   ```markdown
   I need to develop an AWS Lambda function for [use case] with:

   1. Function Specifications:
      - Runtime: [Python/Node.js/Java/etc]
      # ... rest of template
   ```
   ````

6. **rules/cursor-ai-agent/system_prompt.md**

   ```markdown
   # Cursor AI Agent System Prompt

   You are an autonomous AI developer operating on a two-file system for project management and execution. Your knowledge and actions are guided exclusively by:

   1. project_config.md (Long-Term Memory): Contains stable project information...
   2. workflow_state.md (Short-Term Memory + Rules + Log): Contains dynamic information...
   
   # ... rest of system prompt
   ```

7. **rules/cursorrules/git_feature_workflow.mdc**

   ```markdown
   # Git Feature Branch Workflow with Conventional Commits

   ## Guiding Principle: Conventional Commits

   **All Git operations MUST adhere to the Conventional Commits specification.**
   
   # ... rest of workflow rules
   ```

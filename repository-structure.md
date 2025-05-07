# Repository Structure

```plaintext
prompt-atlas/
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
├── guides/
│   └── getting-started.md              # Getting started guide
│
├── prompts/
│   ├── domains/                        # Domain-specific prompts
│   │   ├── cloud/                      # Cloud development
│   │   │   ├── aws-lambda.md
│   │   │   ├── serverless.md
│   │   │   └── architecture.md
│   │   ├── frontend/                   # Frontend development
│   │   │   ├── react.md
│   │   │   ├── components.md
│   │   │   └── performance.md
│   │   ├── backend/                    # Backend development
│   │   │   ├── api.md
│   │   │   ├── database.md
│   │   │   └── microservices.md
│   │   ├── mobile/                     # Mobile development
│   │   │   ├── react-native.md
│   │   │   ├── flutter.md
│   │   │   └── native.md
│   │   └── devops/                     # CI/CD & infrastructure
│   │       └── cicd-and-cloud-integration.md
│   │
│   ├── languages/                      # Language-specific prompts
│   │   ├── python/                     # Python development
│   │   │   ├── python-ai-ml-expert.md
│   │   │   ├── python-simple-optimal-code-prompt.md
│   │   │   └── seasoned-expert-python-ai-ml-swe.md
│   │   ├── typescript/                 # TypeScript development
│   │   │   └── nextjs-expert-dev.md
│   │   └── README.md                   # Overview of language-specific prompts
│   │
│   └── patterns/                       # Common prompt patterns
│       ├── architecture/               # Design patterns
│       ├── optimization/               # Performance patterns
│       ├── testing/                    # Testing patterns
│       └── README.md                   # Overview of prompt patterns
│
├── tools/                              # AI assistant configurations
│   ├── cursor/                         # Cursor AI rules
│   │   └── agent/                      # Autonomous AI agent framework
│   │       └── system_prompt.md
│   ├── chat-models/                    # ChatGPT, Claude, etc.
│   │   └── prompt-engineering/         # Prompt engineering guides
│   │       └── master-prompt-generator.md
│   └── README.md                       # Overview of tools
│
├── rules/
│   ├── cursor-ai-agent/                # Cursor AI Agent framework
│   │   ├── README.md                   # Overview and instructions
│   │   ├── system_prompt.md            # System prompt for Cursor AI
│   │   ├── project_config.md           # Long-term memory template
│   │   └── workflow_state.md           # Short-term memory and rules template
│   │
│   ├── cursorrules/                    # Rules for Cursor AI coding assistant
│   │   └── git_feature_workflow.mdc    # Git feature branch workflow rules
│   │
│   └── copilot/                        # GitHub Copilot optimization
│       ├── instructions/               # Copilot instructions
│       │   ├── chat-agent-mcp-code-instruct-py_2025_05_02.json
│       │   └── chat-codegen-instruct-py_2025_03_13.json
│       └── prompts/                    # Copilot prompts
│           └── mcp-agent-template.prompt.md
│
├── templates/                          # Standardized formats
│   └── prompt-templates/               # Base templates for different categories
│       └── standard-prompt.md          # Standard prompt template
│
├── CONTRIBUTING.md                     # Contribution guidelines
├── LICENSE                             # MIT License
├── README.md                           # Project documentation and overview
└── repository-structure.md             # Repository structure guide
```

## Key Files and Their Contents

1. **README.md**

   - Project overview with badges
   - Feature highlights
   - Repository structure diagram
   - Prompt categories
   - Usage instructions
   - Contribution guidelines
   - License information
   - Author details

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

5. **prompts/domains/cloud/aws-lambda.md**

   ```markdown
   # AWS Lambda Development Prompts

   ## Description

   A collection of prompts for AWS Lambda function development.

   ## Use Cases

   - Serverless function development
   - Event-driven architectures
   - Cloud integration

   # ... rest of content
   ```

6. **tools/cursor/agent/system_prompt.md**

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

8. **templates/prompt-templates/standard-prompt.md**

   ```markdown
   # [Prompt Title]

   ## Description

   A brief description of what this prompt helps accomplish.

   ## Use Cases

   - Primary use case 1
   - Primary use case 2
   - Primary use case 3

   # ... rest of template structure
   ```

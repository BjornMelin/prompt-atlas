# Repository Structure

```plaintext
prompt-atlas/
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   ├── bug_report.md               # Template for bug reports
│   │   └── feature_request.md          # Template for feature requests
│   └── workflows/
│       ├── markdown-lint.yml           # GitHub Action for markdown linting
│       └── mlc_config.json             # Configuration for markdown link checker
│
├── docs/
│   ├── getting-started.md              # Quick start guide for new users
│   └── examples/
│       └── lambda-image-processor.md   # Example implementation
│
├── prompts/                            # AI development prompts organized by tool and domain
│   ├── README.md                       # Overview of prompts directory structure
│   │
│   ├── 🛠️ TOOL-SPECIFIC PROMPTS
│   ├── ai-agents/                      # AI agent development using OpenAI Agents SDK
│   │   └── agent_development_prompt.md # Comprehensive agent development guide
│   │
│   ├── claude-code/                    # Claude Code slash command files
│   │   ├── complete-backend-task.md    # Backend task automation
│   │   ├── complete-frontend-task.md   # Frontend task automation
│   │   ├── complete-highest-todo.md    # General TODO completion
│   │   ├── complete-highest-todo-vect-db.md # Vector database tasks
│   │   ├── complete-integration-task.md # API/Integration tasks
│   │   ├── complete-integration-api-task.md # KISS-focused API tasks
│   │   ├── continue-backend-task.md    # Resume in-progress backend work
│   │   ├── finalize-merge-pr.md        # PR merge finalization
│   │   ├── fix-update-pr.md            # PR update and fixes
│   │   ├── implement-issue.md          # GitHub issue implementation
│   │   ├── issue_completion_refactor.md # Complete TODO/GitHub issues
│   │   ├── iterate-todos.md            # Iterative TODO completion
│   │   ├── phase-implementation.md     # Phased project implementation
│   │   ├── start-pr-review.md          # Pull request review initiation
│   │   └── tripsage-core-prompt.md     # Project-specific core prompt
│   │
│   ├── github-copilot/                 # GitHub Copilot instructions and configs
│   │   └── instructions/               # Copilot instruction files
│   │       ├── chat-agent-mcp-code-instruct-py_2025_05_02.json
│   │       └── chat-codegen-instruct-py_2025_03_13.json
│   │
│   ├── cursor-ai/                      # Cursor IDE rules and configurations
│   │   ├── README.md                   # Cursor AI setup and usage guide
│   │   ├── git_feature_workflow.mdc    # Git workflow rules for Cursor
│   │   ├── project_config.md           # Long-term memory template
│   │   ├── system_prompt.md            # System prompt for Cursor AI
│   │   └── workflow_state.md           # Short-term memory and rules
│   │
│   ├── mcp-servers/                    # Model Context Protocol prompts
│   │   └── mcp-agent-template.prompt.md # MCP agent template
│   │
│   ├── coding-guidelines/              # General coding standards and principles
│   │   └── CLAUDE.md                   # Pragmatic development charter
│   │
│   ├── 🎯 DOMAIN-SPECIFIC PROMPTS
│   ├── backend/                        # Backend development
│   │   ├── api-design.md               # API design patterns
│   │   ├── api.md                      # General API development
│   │   ├── database.md                 # Database design and optimization
│   │   └── microservices.md            # Microservices architecture
│   │
│   ├── frontend/                       # Frontend development
│   │   ├── components.md               # Component design patterns
│   │   ├── performance.md              # Performance optimization
│   │   ├── react-components.md         # React component development
│   │   └── react.md                    # React development patterns
│   │
│   ├── mobile/                         # Mobile development
│   │   ├── flutter.md                  # Flutter development
│   │   ├── native.md                   # Native mobile development
│   │   └── react-native.md             # React Native development
│   │
│   ├── cloud/                          # Cloud development and architecture
│   │   ├── architecture.md             # Cloud architecture patterns
│   │   ├── aws-lambda.md               # AWS Lambda development
│   │   └── serverless.md               # Serverless development
│   │
│   ├── cicd/                           # CI/CD and DevOps
│   │   └── cicd-and-cloud-integration.md # CI/CD pipeline patterns
│   │
│   ├── python/                         # Python development
│   │   ├── python-ai-ml-expert.md      # AI/ML Python expert
│   │   ├── python-expert.md            # General Python expert
│   │   ├── python-simple-optimal-code-prompt.md # Optimal Python patterns
│   │   └── seasoned-expert-python-ai-ml-swe.md # Senior Python AI/ML engineer
│   │
│   ├── typescript/                     # TypeScript development
│   │   └── nextjs-expert-dev.md        # Next.js expert development
│   │
│   └── 🧠 META-PROMPTING
│       └── prompt-engineering/         # Prompt creation and optimization tools
│           ├── master-prompt-generator  # Master prompt generation tool
│           └── master-prompt-generator.xml # XML version of prompt generator
│
├── templates/                          # Standardized formats
│   └── prompt-templates/               # Base templates for different categories
│       └── standard-prompt.md          # Standard prompt template
│
├── .gitignore                          # Git ignore patterns
├── CONTRIBUTING.md                     # Contribution guidelines
├── LICENSE                             # MIT License
├── README.md                           # Project documentation and overview
└── repository-structure.md             # This file - repository structure guide
```

## Organizational Philosophy

The repository is organized around two primary axes:

### 🛠️ Tool-Specific Organization
Prompts are grouped by the AI tool or platform they're designed for:
- **Claude Code**: Slash commands for project automation
- **GitHub Copilot**: Instructions and configurations for enhanced coding assistance
- **Cursor AI**: Rules and workflows for the Cursor IDE
- **AI Agents**: Advanced agent development frameworks
- **MCP Servers**: Model Context Protocol configurations

### 🎯 Domain-Specific Organization  
Technical prompts are organized by development domain:
- **Backend**: APIs, databases, microservices
- **Frontend**: React, components, performance
- **Mobile**: Flutter, React Native, native development
- **Cloud**: AWS, serverless, architecture
- **Languages**: Python, TypeScript specializations

## Key Benefits of This Structure

1. **Tool-First Discovery**: Developers can quickly find prompts for their specific development environment
2. **Domain Expertise**: Easy access to specialized knowledge areas for implementation
3. **Flat Hierarchy**: Minimal nesting reduces navigation complexity
4. **Clear Separation**: Distinct categories prevent overlap and confusion
5. **Scalability**: Easy to add new tools or domains without restructuring

## Usage Patterns

### For Tool-Specific Workflows
```bash
# Find Claude Code commands
prompts/claude-code/

# Set up Cursor AI
prompts/cursor-ai/

# Configure GitHub Copilot
prompts/github-copilot/
```

### For Domain Expertise
```bash
# Backend development guidance
prompts/backend/

# Frontend patterns and optimization
prompts/frontend/

# Python AI/ML development
prompts/python/
```

### For Meta-Prompting
```bash
# Prompt engineering tools
prompts/prompt-engineering/

# General coding guidelines
prompts/coding-guidelines/
```

## File Naming Conventions

- **Tool directories**: Use the tool name (claude-code, cursor-ai, github-copilot)
- **Domain directories**: Use technical domain names (backend, frontend, mobile)
- **Files**: Use descriptive kebab-case names with .md extension
- **Special files**: Configuration files maintain their original extensions (.json, .xml, etc.)

## Migration Notes

This structure represents a complete reorganization from the previous version:
- Former `rules/` content moved to tool-specific directories
- Former `tools/` content integrated into appropriate categories  
- Domain structure flattened from nested `domains/languages/` to top-level
- Clear separation between tool-specific and domain-specific content

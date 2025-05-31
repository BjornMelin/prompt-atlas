# Claude Code Slash Commands Directory

This directory contains a comprehensive collection of slash commands for Claude Code, organized into logical categories for easy navigation and use.

## Directory Structure

### 📋 Issue & Task Management
Commands for managing GitHub issues and project tasks.

- [`implement-issue.md`](issue-task-management/implement-issue.md) - Complete implementation of a specific GitHub issue
- [`resolve-priority-issue.md`](issue-task-management/resolve-priority-issue.md) - Resolve the highest priority GitHub issue with comprehensive approach
- [`complete-highest-todo.md`](issue-task-management/complete-highest-todo.md) - Complete the highest priority TODO item
- [`complete-highest-todo-vect-db.md`](issue-task-management/complete-highest-todo-vect-db.md) - Complete highest priority vector database TODO
- [`iterate-todos.md`](issue-task-management/iterate-todos.md) - Systematically work through TODO items
- [`issue_completion_refactor.md`](issue-task-management/issue_completion_refactor.md) - Refactor and complete issue resolution

### 🔧 Development Tasks
Commands for specific development work and implementation.

- [`complete-backend-task.md`](development-tasks/complete-backend-task.md) - Complete highest priority backend task
- [`complete-frontend-task.md`](development-tasks/complete-frontend-task.md) - Complete highest priority frontend task
- [`continue-backend-task.md`](development-tasks/continue-backend-task.md) - Continue working on backend tasks
- [`phase-implementation.md`](development-tasks/phase-implementation.md) - Implement specific project phases

### 🌿 Branch Management
Commands for Git branch operations and workflows.

- [`start-branch-review.md`](branch-management/start-branch-review.md) - Begin comprehensive review of a Git branch
- [`fix-update-branch.md`](branch-management/fix-update-branch.md) - Fix and update branch based on review feedback
- [`finalize-merge-branch.md`](branch-management/finalize-merge-branch.md) - Finalize and merge branch to main

### 🔀 Pull Request Management
Commands for GitHub pull request workflows.

- [`start-pr-review.md`](pull-request-management/start-pr-review.md) - Start pull request review process
- [`fix-update-pr.md`](pull-request-management/fix-update-pr.md) - Fix and update pull request
- [`finalize-merge-pr.md`](pull-request-management/finalize-merge-pr.md) - Finalize and merge pull request

### 🔍 Code Review & Quality
Commands for code review and quality assurance.

- [`comprehensive-code-review.md`](code-review-quality/comprehensive-code-review.md) - Conduct complete expert-level repository review and alignment

### 📖 General Guidelines
General purpose commands and implementation guidelines.

- [`general-task-prompt.md`](general-guidelines/general-task-prompt.md) - General task implementation with comprehensive guidelines
- [`implementation-guidelines.md`](general-guidelines/implementation-guidelines.md) - Core implementation guidelines and tool usage
- [`advanced-implementation-guide.md`](general-guidelines/advanced-implementation-guide.md) - Advanced implementation guidelines with detailed tool usage
- [`tripsage-core-prompt.md`](general-guidelines/tripsage-core-prompt.md) - TripSage specific core prompt

## Usage

To use any of these slash commands in Claude Code:

1. Navigate to the appropriate subdirectory based on your task type
2. Use the command file name (without the `.md` extension) as your slash command
3. Add any required arguments after the command name

### Example Usage

```bash
# Use a general task command with arguments
/general-task-prompt "Implement user authentication system"

# Use an issue resolution command
/resolve-priority-issue 

# Use a branch review command with branch name
/start-branch-review "feat/user-auth-system"
```

## Command Categories Explained

- **Issue & Task Management**: Best for structured project work, GitHub issue resolution, and TODO management
- **Development Tasks**: Ideal for specific backend/frontend development work and phase-based implementation
- **Branch Management**: Perfect for Git workflow management and branch-specific operations
- **Pull Request Management**: Essential for GitHub PR workflows and code review processes
- **Code Review & Quality**: Comprehensive tools for code quality assessment and repository alignment
- **General Guidelines**: Foundational commands and implementation patterns for all types of development work

## Contributing

When adding new slash commands:

1. Follow the existing file structure with proper `$ARGUMENTS` placeholder
2. Place commands in the most appropriate subdirectory
3. Update this README.md file with the new command
4. Ensure command names are descriptive and follow the existing naming conventions

## File Format

All slash command files follow this structure:

```markdown
# Command Title

[Command description and instructions]

[Optional sections with guidelines, best practices, etc.]

$ARGUMENTS
```

The `$ARGUMENTS` placeholder allows users to pass custom arguments to the command when executed.
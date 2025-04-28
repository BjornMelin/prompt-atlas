# Feature: Ultimate Cursor AI Agent Template

## Description

This PR adds a comprehensive template for creating autonomous AI agents in Cursor IDE. It introduces a structured, two-file system that enables AI assistants to maintain context, follow software engineering best practices, and automate development workflows.

The template is inspired by and combines the best practices from:
- [Bhartendu-Kumar/rules_template](https://github.com/Bhartendu-Kumar/rules_template)
- [kleosr/cursorkleosr](https://github.com/kleosr/cursorkleosr)

## Changes

- **Added new directory**: `rules/cursor-ai-agent/` containing:
  - `README.md`: Comprehensive guide with features, implementation instructions, and best practices
  - `system_prompt.md`: Instructions for Cursor AI on how to operate with the two-file system
  - `project_config.md`: Template for long-term project memory (LTM)
  - `workflow_state.md`: Template for dynamic workflow state tracking (STM)

- **Updated main README.md**:
  - Added section for AI Tools & Rules
  - Added table of contents
  - Added How to Cite section with BibTeX citation
  - Updated badges and features
  - Improved structure and content organization

- **Updated repository-structure.md**:
  - Added new directory and files to the structure diagram
  - Added description of key files in the new directory

## Implementation Details

The template implements an autonomous workflow loop:
1. **READ**: AI reads workflow_state.md to understand current context
2. **INTERPRET**: AI determines actions based on state and rules
3. **ACT**: AI executes actions using Cursor tools
4. **UPDATE**: AI records actions and updates state
5. **REPEAT**: Cycle continues until task completion

Development follows a structured four-phase process:
- **ANALYZE**: Understand requirements thoroughly
- **BLUEPRINT**: Create detailed implementation plan (requires user approval)
- **CONSTRUCT**: Execute plan with proper error handling
- **VALIDATE**: Test implementation against requirements

## How to Use

Full instructions are provided in the `rules/cursor-ai-agent/README.md` file, including:
- File structure setup
- Configuration steps
- MCP tool integration
- Workflow operation
- Best practices

## Why This Matters

This template provides several benefits for AI-assisted development:
- Increases autonomy while maintaining human oversight at critical points
- Ensures consistent application of software engineering principles
- Manages context efficiently across complex tasks
- Prevents "drift" during iterative processing
- Integrates with MCP tools for enhanced capabilities

## Related Issues

N/A

## Screenshots

N/A

## Checklist
- [x] I have followed the repository's contribution guidelines
- [x] I have added necessary documentation
- [x] I have updated the repository structure documentation
- [x] I have tested the template functionality

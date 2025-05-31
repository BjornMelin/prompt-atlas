## Resolve Highest Priority GitHub Issue

**Prioritize clear, maintainable, and efficient code and organization, delivering robust, fully featured, and best-practice solutions without unnecessary complexity.  
Do NOT support or maintain backwards compatibility—completely replace legacy solutions with modern, best-practice implementations. Use only Pydantic 2.x for new models. Always aim for 80%+ testing coverage of the code completed for this issue.**

### Reference Documentation & System Alignment

- **Before starting, deeply review all project documentation—especially `@docs/REFACTOR/`—to ensure full alignment with the current system design.**
- When unsure about architecture, implementation details, or file relevance, always refer to the latest `@docs/REFACTOR/` files for clarification.
- **Proactively identify, flag, and remove any outdated, deprecated, or unused files, modules, or features** that do not match the updated architecture or are called out as obsolete in the refactor docs.
- Keep all project docs up to date as you make changes, and reference relevant documentation throughout your work.

### Issue Resolution Workflow

1. **Gather Context**
   - Use `github_issue_fetch` (MCP) to retrieve full GitHub issue details.
   - Deeply review the issue description, comments, attachments, and all relevant documentation, with particular focus on `@docs/REFACTOR/`.
   - If any functionality, file, or API seems unclear or possibly outdated, cross-check it with `@docs/REFACTOR/` and clean it up if appropriate.
   - Update project docs if you clarify, change, or remove any features.

2. **Planning and Subtask Breakdown**
   - Explore and understand the current implementation using file reading tools and `context7`.
   - Use "think hard" or "ultrathink" for complex issues.
   - Break the work into a clear, actionable markdown checklist using the built-in TODO tool. Track progress visibly.
   - For complex issues, use `sequential-thinking` for a step-by-step execution plan.
   - Justify your plan and approach for each subtask using best practices, documentation, and direct references to `@docs/REFACTOR/`.

3. **Parallel Tool-Driven Research, Implementation, and Automation**
   - Throughout all phases, use all relevant MCP server tools for research, code, testing, automation, and documentation.
   - Select the most relevant tools for each step—see MCP Server Tool Usage Guide below.
   - Use tools in parallel wherever possible for speed and thoroughness.

4. **Review and Sub-Agent Verification**
   - After implementation, spawn a sub-agent for independent review—focus on code quality, maintainability, edge cases, error handling, performance, and security.
   - Address all sub-agent feedback and iterate as needed.

5. **Branch, Implement, Test, and Clean Up**
   - Create a new branch using conventional-commits format (e.g., `git checkout -b feat/issue-456-user-auth`).
   - Implement all required changes, focusing on maintainability, clarity, and completeness.
   - **Remove or refactor any temporary, obsolete, or legacy files and code that are no longer needed or do not fit the updated system design.**
   - Build or update the test suite for all new/changed code. Ensure at least 80% testing coverage. Run `uv pytest` to verify all tests pass.
   - Always run `uv ruff lint` and `uv ruff format` on all worked files. **Fix all issues before committing or opening a PR.**

6. **Document, Monitor Progress, and Wrap Up**
   - Update all relevant documentation, READMEs, and project docs (especially `@docs/REFACTOR/`) to reflect the latest changes, progress, and design decisions.
   - Commit and push changes. Open a PR via GitHub MCP server tools (not local CLI).
   - **STOP HERE** — Do not merge; use the PR review/merge command next.

7. **Final Output & Reporting**
   - Summarize unresolved questions, ambiguities, or next steps.
   - Output a logical summary including:
     - The new branch name
     - Checklist of completed subtasks
     - Key changes, design decisions, and supporting reference links
     - Any blockers, open questions, or next steps
   - Justify all major decisions with research, best practices, and references to `@docs/REFACTOR/`.
   - Keep reference links handy for rapid documentation lookups.

## Best Practices and Quality Triggers
- Use parallel tool calls wherever possible for efficiency and coverage.
- Always align implementation and cleanup with the latest `@docs/REFACTOR/` architecture.
- Create a markdown checklist for all steps; check off as completed.
- Spawn a sub-agent for code review and improvements.
- Justify major decisions with best practices and documentation.
- Keep reference links handy for optimal implementation.

## MCP Server Tool Usage Guide

- **supabase:** For all database-related operations (`SUPABASE_PROJECT_ID=uzqcjksjeoupwzkfhreo`).
- **repomix:** For repo summarization, packing/unpacking, merges, analysis, and automated code manipulation.
- **github:** For GitHub actions—issue/PR creation, commenting, status checks, and review automation.
- **git:** For local git operations—branching, commits, diffs, merges, reverts, logs, tagging, etc.
- **linkup, exa, tavily, firecrawl_scrape, firecrawl_crawl, firecrawl_deep_research, context7, sequential-thinking:** For research, planning, docs, codebase understanding, web lookups, and code/architecture plans.
- **playwright:** For automated browser actions (integration/UI testing, web scraping/verification).
- **time:** For date/time automation or simulation.
- **google-maps:** For geo-location/mapping if relevant.
- **Always use the most appropriate tool for the task at hand—across research, planning, code, automation, testing, or docs. Invoke tools in parallel wherever possible for speed and coverage.**

$ARGUMENTS
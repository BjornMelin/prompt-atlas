## Goal
Prioritize clear, maintainable, and efficient code and organization, delivering robust, fully featured, and best-practice solutions without unnecessary complexity. Solutions should be simple, yet powerful and comprehensive.

## Instructions

### Issue: $ARGUMENTS

1. Context Gathering and Analysis
- Use the `github_issue_fetch` MCP server tool to retrieve the complete details, comments, and attachments for the provided GitHub issue number.
- For codebase exploration, use the built-in file reading tool and `context7` to collect, analyze, and reference relevant code, configuration, and documentation files.
- For web research, use `exa` for accurate and reliable web searches, and use `tavily` or `linkup` as supplemental web search and best-practice discovery tools.
- For documentation gathering, use `firecrawl_scrape` and `firecrawl_crawl` to extract and crawl official documentation and project docs. Use `firecrawl_deep_research` for in-depth investigation of complex or broad topics.
- Review all relevant official docs, community examples, and project documentation for context. Reference and update project docs as you progress.

2. Planning and Subtask Breakdown
- Explore and understand the current implementation before writing any code, using the file reading tool and `context7` as needed.
- Use "think hard" or "ultrathink" for complex or multi-step issues.
- Break the task into a clear, actionable markdown checklist using the built-in TODO tool. Track and mark progress as you complete each subtask.
- For complex issues, use `sequential-thinking` to generate a systematic, step-by-step execution plan.
- For each subtask, plan and justify your approach based on research, best practices, and documentation. Reference relevant files and sources.

3. Local Branching, Implementation, and Testing (Command Line & gh CLI)
- In the terminal, use Bash commands and the `gh` CLI for all local git operations.
    - Create a new branch using the conventional commits format (e.g., `feat/issue-456-user-auth`):  
      `git checkout -b feat/issue-456-user-auth`
    - Stage changes:  
      `git add .`
    - Commit with a clear, conventional message referencing the issue:  
      `git commit -m "feat(issue-456): [concise description of changes]"`
    - Push the branch to the remote repository:  
      `git push -u origin feat/issue-456-user-auth`
- Implement all required changes in the new branch, focusing on maintainability, clarity, and feature-completeness according to the stated goal above.
- Remove all temporary scripts or helper files before considering the task complete.
- Build or update the test suite for all new or changed code. Run `uv pytest` to verify all tests pass.
- Always run `uv ruff lint` and `uv ruff format` on all files you worked on. Fix all linting and formatting issues before committing or opening a PR.

4. Review and Sub-Agent Verification
- After implementation, use the sub-agent verification pattern: spawn a sub-agent to independently review the code for issues, edge cases, error handling, performance, and security.
- Address all sub-agent feedback and iterate as needed.

5. Documentation, TODOs, and Progress Monitoring
- When all TODO subtasks are complete, update `@TODO.md` to reflect completion and add new or follow-up tasks as identified.
- Update all relevant documentation, README files, and project docs to reflect the changes, progress, and important design decisions.
- Summarize and structure outputs logically, with referenced decisions and justifications.

6. Pull Request (MCP Server Tool)
- Use the GitHub MCP server tools to create and manage pull requests (not local CLI).  
- Stop here; do not merge until PR review and merge steps are run separately.
- Output a summary of:
    - The new branch name
    - Checklist of completed subtasks
    - Key changes, design decisions, and any supporting reference links
    - Any blockers, open questions, or next steps

## Best Practices and Quality Triggers
- Use parallel tool calls wherever possible to maximize efficiency and coverage.
- For maximum efficiency, whenever you need to perform multiple independent operations, invoke all relevant tools simultaneously rather than sequentially.
- Think hard about the requirements and create a detailed plan before coding.
- First explore, then think hard and plan, then implement, then commit.
- Create a markdown checklist breaking down all required steps. Work through each item systematically, checking them off as completed.
- Spawn a sub-agent to independently review this for issues and improvements.
- Justify all major decisions with research and/or best practices.
- Keep reference links handy for rapid documentation lookups and optimal implementation.

## MCP Server Tool Usage Guide
- `github_issue_fetch` (MCP): Fetch issue details, comments, and attachments.
- Built-in file reading tool: Codebase and project file exploration.
- `context7`: Retrieve and analyze relevant code and documentation.
- `exa`: Accurate, reliable web search.
- `firecrawl_scrape`: Scrape documentation and referenced links for details.
- `firecrawl_crawl`: Crawl documentation sites for deeper, related content.
- `firecrawl_deep_research`: Conduct deep research on complex or broad topics.
- `tavily`, `linkup`: Web searches for community best practices.
- `sequential-thinking`: Systematically plan and reason through complex issues.
- Command line & gh CLI:  
    - `git checkout -b [branch]`  
    - `git add .`  
    - `git commit -m "[conventional message]"`  
    - `git push -u origin [branch]`
- GitHub MCP PR tools: Create and manage pull requests.

## Example Input
Implement the requirements described in GitHub issue #456.

## Final Reminders
- Follow all instructions and best practices above.  
- Begin by gathering full context, then "think hard" and plan, create a new branch using conventional commits, fully implement, test, validate, and output a summary with a checklist and branch details. Use parallel tool calls wherever possible. Spawn a sub-agent for code review, clean up all temporary files, and update documentation and TODOs as needed.

## Complete Highest Priority TODO or GitHub Issue

**Prioritize clear, maintainable, and efficient code and organization, delivering robust, fully featured, and best-practice solutions without unnecessary complexity. Solutions should be simple, yet powerful and comprehensive.  
Do NOT support or maintain backwards compatibility—completely replace legacy solutions with modern, best-practice implementations. Use only Pydantic 2.x for new models. Always aim for 80%+ testing coverage of the code completed for this issue.**

### Reference Documentation  
- **Before starting, deeply review all documentation in `@docs/REFACTOR/` to determine what to implement, and refer back to these docs throughout your work. If you forget details or need clarification during the process, check these docs first.**
- For quick library or code example lookups, always check with `context7` before using further MCP server tools for deeper exploration.

### Task Workflow

1. **Gather Context**
   - **If working from a GitHub issue:**  
     - Use `github_issue_fetch` (MCP) to retrieve full issue details.
     - Deeply review the issue description, all comments, and attachments, as well as all relevant project documentation.
     - Cross-reference the requirements and goals of the GitHub issue with the current tasks in `@TODO.md` to ensure that the TODO list accurately reflects all outstanding work related to the issue before starting.
   - **If working directly from `@TODO.md` (no issue specified):**  
     - Select the single highest-priority main entry or feature to implement next.
     - Cross-reference each selected TODO task with the docs in `@docs/REFACTOR/` and other related project documentation in `@docs/` to ensure full context and alignment before starting.
   - In all cases, review and update project docs as you progress.

2. **Planning and Subtask Breakdown**
   - Explore and understand the current implementation before writing any code, using the file reading tool and `context7` as needed.
   - Use "think hard" or "ultrathink" for complex or multi-step issues.
   - Break the task into a clear, actionable markdown checklist using the built-in TODO tool. Track and mark progress as you complete each subtask.
   - For complex issues, use `sequential-thinking` to generate a systematic, step-by-step execution plan.
   - For each subtask, plan and justify your approach based on research, best practices, and documentation. Reference relevant files and sources.

3. **Parallel Tool-Driven Research, Implementation, and Automation**
   - Throughout research, planning, implementation, automation, testing, and documentation, **use all available MCP server tools as needed** to maximize efficiency and code quality.
   - For each step, select the most relevant tools for the task (see the MCP Server Tool Usage Guide below for full details).
   - For example, use `context7`, `firecrawl_scrape`, `firecrawl_crawl`, `firecrawl_deep_research`, `exa`, `tavily`, `linkup`, `repomix`, `github`, `git`, `supabase`, and others, as appropriate.
   - Always use tools in parallel wherever possible for speed and coverage.

4. **Review and Sub-Agent Verification**
   - After implementation, use the sub-agent verification pattern: spawn a sub-agent to independently review the code for issues, edge cases, error handling, performance, and security.
   - Address all sub-agent feedback and iterate as needed.

5. **Branch, Implement, and Test**
   - Create a new branch using conventional-commits format (e.g., `git checkout -b feat/issue-456-user-auth`).
   - Implement all required changes, focusing on maintainability, clarity, and completeness.
   - Remove any temporary scripts or helper files before considering the task complete.
   - Build or update the test suite for all new or changed code. **Ensure at least 80% testing coverage for the code completed in this issue.** Run `uv pytest` to verify all tests pass.
   - Always run `uv ruff lint` and `uv ruff format` on all files worked on. **Fix all linting/formatting issues before committing or opening a PR.**

6. **Document, Monitor Progress, and Wrap Up**
   - Once all TODO tool subtasks are complete, update `@TODO.md` to reflect completion and add new/follow-up tasks as identified.
   - Update all relevant documentation, READMEs, and project docs to reflect changes, progress, and design decisions.
   - Commit and push changes. Open a PR via the GitHub MCP server tools (do not use local CLI for PRs).
   - **STOP HERE** — Do not merge; use the PR review/merge command next.

7. **Final Output & Reporting**
   - Summarize unresolved questions, ambiguities, or next steps.
   - Output a logical summary including:
     - The new branch name
     - Checklist of completed subtasks
     - Key changes, design decisions, and supporting reference links
     - Any blockers, open questions, or next steps
   - Justify all major decisions with research or best practices.
   - Keep reference links handy for rapid documentation lookups.

## Best Practices and Quality Triggers
- **Use parallel tool calls wherever possible to maximize efficiency and coverage.**
- Whenever you need to perform multiple independent operations, invoke all relevant tools simultaneously rather than sequentially.
- Think hard about the requirements and create a detailed plan before coding.
- First explore, then think hard and plan, then implement, then commit.
- Create a markdown checklist breaking down all required steps. Work through each item systematically, checking them off as completed.
- Spawn a sub-agent to independently review for issues and improvements.
- Justify all major decisions with research and/or best practices.
- Keep reference links handy for rapid documentation lookups and optimal implementation.

## MCP Server Tool Usage Guide

- **supabase:** For all database-related operations in your Supabase project (configure with your project ID).
- **repomix:** For advanced repo operations—summarization, packing/unpacking, code merges, analysis, and automated code manipulation.
- **github:** For all GitHub actions—issue and PR creation/updates, commenting, status checks, automation of review processes.
- **git:** For local git operations—branching, commits, diffs, merges, reverts, logs, tagging, etc.
- **linkup, exa, tavily, firecrawl_scrape, firecrawl_crawl, firecrawl_deep_research, context7, sequential-thinking:** For research, planning, up-to-date docs, codebase understanding, deep web lookups, stepwise reasoning, and generating code/architecture plans.
- **playwright:** For automated browser actions (integration/UI testing, web scraping/verification, automation of browser workflows).
- **time:** For time/date-related automation or simulation (e.g., logging, scheduled actions, test time manipulation).
- **google-maps:** For geo-location lookups, maps, routing, or related data (include only if relevant to the project).
- **Always use the most appropriate tool for the task at hand—across research, planning, code implementation, automation, testing, or documentation. Invoke tools in parallel wherever possible for speed and coverage.**

$ARGUMENTS
## Continue and Complete Current Implementation Phase (TripSage Project)

**Prioritize clear, maintainable, and efficient code and organization, delivering robust, fully featured, and best-practice solutions without unnecessary complexity. Solutions should be simple, yet powerful and comprehensive.**

1. Read `@PHASE_5_IMPLEMENTATION_PROMPT.md` and follow the prompt provided, completing all tasks as laid out in the file.
2. Use MCP server tools as needed for research, planning, and execution:
   - `tavily`, `exa`, `linkup`: For web search, codebase exploration, and external resource lookups.
   - `firecrawl_scrape`, `firecrawl_crawl`, `firecrawl_deep_research`: To crawl, scrape, and research documentation or examples.
   - `context7`: To retrieve the latest library and package versions, code examples, and to ensure compatible versions/dependencies.
   - `sequential-thinking`: For systematic planning, deep thinking, or breaking down complex/ambiguous requirements.
3. Track your progress and completion in all appropriate project files: `@TODO.md`, `@tasks/TODO-INTEGRATION.md`, `@tasks/TODO-API.md`, and `@PHASE_4_IMPLEMENTATION_PROMPT.md`. Update these files as tasks are completed or requirements evolve.
4. Actively use your built-in TODO tool to break down the phase's tasks into actionable subtasks. Manage and mark progress as you work, and sync completed subtasks to the relevant TODO/project files.
5. If all phase tasks are complete:
   - Delete the `@PHASE_4_IMPLEMENTATION_PROMPT.md` file.
   - Write a detailed next prompt for phase 5.
   - If there is no further phase (work is done), review `@TODO.md`, `@tasks/TODO-API.md`, and `@tasks/TODO-INTEGRATION.md` to create a new phased plan and set of detailed prompt files for the next core API/Integration related highest-priority tasks to complete—following the style, structure, and best practices of previous phase prompt files.
6. Once the next phase prompt(s) and updated TODO/project files are set, commit and push all changes to remote.
7. Use the GitHub MCP tools to create a new pull request for these changes.
8. **STOP HERE** — Do not merge; use your PR review/merge command next.
9. **Final reminders:** Summarize any unresolved questions, ambiguities, or next steps; ensure all outputs are structured logically with actionable details and referenced decisions; justify major decisions with research and/or best practices; keep reference links handy for rapid doc lookups and optimal solutions.

---
### Reference Docs:
- FastAPI: https://fastapi.tiangolo.com/
- Pydantic V2: https://docs.pydantic.dev/latest/
- OpenAI Agents SDK: https://openai.github.io/openai-agents-python/
- FastMCP 2.0: https://gofastmcp.com/getting-started/welcome
- Model Context Protocol: https://modelcontextprotocol.io/introduction
- Playwright: https://playwright.dev/docs/intro
- Playwright MCP: https://github.com/executeautomation/mcp-playwright
- Stagehand MCP: https://github.com/browserbase/stagehand
- Redis MCP: https://github.com/modelcontextprotocol/servers/tree/main/src/redis
- Postgres MCP: https://github.com/modelcontextprotocol/servers/tree/main/src/postgres
- SQLite MCP: https://github.com/modelcontextprotocol/servers/tree/main/src/sqlite
- Browserbase MCP: https://github.com/browserbase/mcp-server-browserbase/tree/main/browserbase
- Firecrawl MCP Server: https://github.com/mendableai/firecrawl-mcp-server
- Google Calendar MCP: https://github.com/nspady/google-calendar-mcp
- OpenAPI MCP Server: https://github.com/janwilmake/openapi-mcp-server
- OWASP: https://owasp.org/

$ARGUMENTS

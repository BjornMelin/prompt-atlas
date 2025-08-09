## Continue Backend Task (In Progress)

**Prioritize clear, maintainable, and efficient code and organization, delivering robust, fully featured, and best-practice solutions without unnecessary complexity. Solutions should be simple, yet powerful and comprehensive.**

1. Continue work on the current phases tasks that are in progress. Resume the subtasks you previously broke down using your built-in TODO tool.
2. Review and update your actionable subtasks as needed in your built-in TODO tool. Actively manage and mark these as you work.
3. Reference all relevant official docs, community examples, and project documentation below for context. Keep project docs updated as you implement.
4. Use MCP server tools as needed for research and implementation:
   - `firecrawl_scrape`: Scrape/extract content from official docs and reference links.
   - `firecrawl_crawl`: Crawl doc sites for deeper or related content.
   - `firecrawl_deep_research`: For in-depth research on complex or broad topics.
   - `context7`: Fetch, read, and analyze API/library docs for examples/usage.
   - `exa`: For codebase exploration/static analysis.
   - `tavily`, `linkup`: For web search and community patterns if official docs lack detail.
   - `sequential-thinking`: For systematic reasoning or complex planning.
5. Plan and justify your approach for each subtask, based on research, best practices, and documentation.
6. Continue implementation on your existing branch (conventional-commits format). Focus on maintainability, clarity, and feature-completeness.
7. Build or update the test suite for all new/changed backend code. Run `uv pytest` and ensure all tests pass.
8. Always run `uv ruff lint` and `uv ruff format` on all files worked on. **Fix all linting/formatting issues before committing or submitting a PR.**
9. Once all TODO tool subtasks for this task are complete, update the `@TODO.md` and specific other TODO and docs to reflect completion, and add new/follow-up tasks if needed.
10. Update all relevant documentation, READMEs, and project docs to reflect changes, progress, and design decisions.
11. Commit and push changes. Open a PR via GitHub MCP server tools.
12. **STOP HERE** — Do not merge; use your PR review/merge command next.
13. **Final reminders:** Summarize any unresolved questions, ambiguities, or next steps; structure outputs logically with actionable details and referenced decisions; justify all major decisions with research and/or best practices; keep reference links handy for rapid doc lookups and optimal solutions.

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

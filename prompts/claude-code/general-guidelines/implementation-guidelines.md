**Implementation Guidelines & Tool Usage**

Leverage all available MCP server tools to ensure robust, efficient, and best-practice solutions. Use the latest versions and dependencies throughout.

---

### Core Principles

- Prioritize clear, maintainable, and efficient code and organization.
- Deliver robust, comprehensive solutions—avoid unnecessary complexity.
- Fully replace legacy code; do not maintain backwards compatibility.
- Use **Pydantic 2.x** exclusively for new models.
- Target **80%+ test coverage** for all completed code.

---

### Tool-Driven Research & Development

- Start documentation and example lookups with `context7`.
- If more depth is needed, expand with:
  - `tavily`, `exa`, `linkup`: For broad web search and community discussions.
  - `firecrawl_scrape`, `firecrawl_crawl`, `firecrawl_extract`, `firecrawl_deep_research`: To scrape/crawl/extract from official docs or for deep investigation.
- Use tools **in parallel** wherever possible for maximum efficiency.

---

### Best Practices

- Plan thoroughly before coding: Explore, plan, implement, then commit.
- Create a markdown checklist for all required steps and work through it systematically.
- Spawn a sub-agent to independently review the work for issues/improvements.
- Justify all major decisions with research and/or best practices.
- Keep key reference links handy for rapid lookups.

---

### Official Documentation (Priority Sources)

Start with `context7` for latest docs, code, and updates. If needed, use `tavily`, `exa`, `linkup` for wider web/community search or `firecrawl_*` tools for deep scraping/extraction.

#### Core Services & Libraries
- **Pydantic V2:** https://docs.pydantic.dev/latest/
- **DragonflyDB:** https://www.dragonflydb.io/docs/
- **OWASP:** https://owasp.org/
- **LangGraph:** https://langchain-ai.github.io/langgraph/
- **Model Context Protocol:** https://modelcontextprotocol.io/introduction
- **Playwright:** https://playwright.dev/docs/intro
- **Crawl4AI:** https://docs.crawl4ai.com/
- **Mem0:** https://docs.mem0.ai/overview

#### APIs and SDKs
- **OpenAI API:** https://platform.openai.com/docs/api-reference/introduction
- **OpenAI Python SDK:** https://github.com/openai/openai-python/blob/main/api.md
- **Supabase:** https://supabase.com/docs
- **Google Maps Platform:** https://developers.google.com/maps/documentation
- **Google Maps Python SDK:** https://github.com/googlemaps/google-maps-services-python
- **Google Calendar API:** https://developers.google.com/workspace/calendar/api/guides/overview
- **Google Calendar Python Quickstart:** https://developers.google.com/workspace/calendar/api/quickstart/python
- **Duffel Flights API:** https://duffel.com/docs/api/overview/welcome
- **OpenWeatherMap API:** https://openweathermap.org/api

#### Notable Mentions
- **Python `time` Library:** https://docs.python.org/3/library/time.html

---

### MCP Server Tool Guide

- **supabase**: Use for all database operations (`SUPABASE_PROJECT_ID=uzqcjksjeoupwzkfhreo`).
- **repomix**: For repo summarization, packing, code merges, and automated analysis/manipulation.
- **github**: For all GitHub issue/PR actions and review automation.
- **git**: For local version control—branching, diffs, merges, etc.
- **linkup, exa, tavily, firecrawl_scrape, firecrawl_crawl, firecrawl_extract, firecrawl_deep_research, context7, sequential-thinking**: For research, planning, up-to-date docs, deep web lookups, codebase understanding, and architectural planning.
- **playwright**: For browser automation, integration/UI testing, and workflow automation.
- **time**: For time/date-related automation or simulation.
- **google-maps**: For geo-location and mapping, if relevant.

**Always select the most suitable tool for the job—across research, planning, implementation, automation, testing, and documentation. Use parallel tool calls to maximize speed and coverage.**

$ARGUMENTS
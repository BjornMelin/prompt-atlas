**Implementation Guidelines and Tool Usage**

Be sure to leverage all available MCP server tools as needed to ensure you have the best possible implementation, using the latest versions and dependencies.

**Core Principles**
- Prioritize clear, maintainable, and efficient code and organization.
- Deliver robust, fully featured, and best-practice solutions without unnecessary complexity.
- Solutions should be simple, yet powerful and comprehensive.
- Do **not** support or maintain backwards compatibility—completely replace legacy solutions with modern, best-practice implementations.
- Use **only Pydantic 2.x** for new models.
- Always aim for **80%+ testing coverage** of the code completed for this issue.

---

**Parallel Tool-Driven Research**
- For library and example documentation, always start with `context7` to retrieve the latest docs, code examples, and updates.
- If additional research or deeper information is required, expand your search using:
    - `tavily`, `exa`, `linkup`: For broad web search, community discussions, and external resources.
    - `firecrawl_scrape`, `firecrawl_crawl`, `firecrawl_extract`, `firecrawl_deep_research`: To scrape, crawl, and extract from official docs or conduct deep technical investigation.
- Use the following MCP server tools in **parallel** wherever possible to gather information efficiently:
    - `firecrawl_scrape`: Scrape and extract content from official docs and reference links.
    - `firecrawl_crawl`: Crawl doc sites for broader or deeper related content.
    - `firecrawl_deep_research`: For in-depth, complex, or broad technical investigation.
    - `exa`: For accurate, reliable web search and codebase exploration.
    - `tavily`, `linkup`: For web search and community best practices if official docs lack details.

---

## Best Practices and Quality Triggers

- Use **parallel tool calls** wherever possible to maximize efficiency and coverage.
- When you need to perform multiple independent operations, invoke all relevant tools **simultaneously** rather than sequentially.
- Think deeply about the requirements and create a detailed plan before coding.
- First explore, then plan thoroughly, then implement, then commit.
- Create a markdown checklist breaking down all required steps. Work through each item systematically, checking them off as completed.
- Spawn a sub-agent to independently review for issues and improvements.
- Justify all major decisions with research and/or best practices.
- Keep reference links handy for rapid documentation lookups and optimal implementation.

---

## Official Documentation Reference Sites

When researching, scraping, crawling, or referencing documentation, use these official sources as a priority.

- **For the latest documentation, code examples, and updates:**  
  First check with `context7`.  
  If additional information or deeper research is needed, expand your search using:
    - `tavily`, `exa`, `linkup` — for broad web search, community discussions, and external resources.
    - `firecrawl_scrape`, `firecrawl_crawl`, `firecrawl_extract`, `firecrawl_deep_research` — to scrape, crawl, and extract from official docs, or conduct deep technical investigation.

### Core Services & Libraries

- **Pydantic V2:** [https://docs.pydantic.dev/latest/](https://docs.pydantic.dev/latest/)
- **DragonflyDB:** [https://www.dragonflydb.io/docs/](https://www.dragonflydb.io/docs/)
- **OWASP:** [https://owasp.org/](https://owasp.org/)
- **LangGraph:** [https://langchain-ai.github.io/langgraph/](https://langchain-ai.github.io/langgraph/)
- **Model Context Protocol (MCP):** [https://modelcontextprotocol.io/introduction](https://modelcontextprotocol.io/introduction)
- **Playwright:** [https://playwright.dev/docs/intro](https://playwright.dev/docs/intro)
- **Crawl4AI:** [https://docs.crawl4ai.com/](https://docs.crawl4ai.com/)
- **Mem0:** [https://docs.mem0.ai/overview](https://docs.mem0.ai/overview)

### APIs and SDKs

- **OpenAI API:** [https://platform.openai.com/docs/api-reference/introduction](https://platform.openai.com/docs/api-reference/introduction)
- **OpenAI Python SDK API:** [https://github.com/openai/openai-python/blob/main/api.md](https://github.com/openai/openai-python/blob/main/api.md)
- **Supabase:** [https://supabase.com/docs](https://supabase.com/docs)
- **Google Maps Platform:** [https://developers.google.com/maps/documentation](https://developers.google.com/maps/documentation)
- **Google Maps Python SDK:** [https://github.com/googlemaps/google-maps-services-python](https://github.com/googlemaps/google-maps-services-python)
- **Google Calendar API:** [https://developers.google.com/workspace/calendar/api/guides/overview](https://developers.google.com/workspace/calendar/api/guides/overview)
- **Google Calendar API Python Quickstart:** [https://developers.google.com/workspace/calendar/api/quickstart/python](https://developers.google.com/workspace/calendar/api/quickstart/python)
- **Duffel Flights API:** [https://duffel.com/docs/api/overview/welcome](https://duffel.com/docs/api/overview/welcome)
- **OpenWeatherMap API:** [https://openweathermap.org/api](https://openweathermap.org/api)

### Notable Mentions

- **Time Library:** *(Standard Python Library, [Docs](https://docs.python.org/3/library/time.html))*

---

## MCP Server Tool Usage Guide

- **supabase:** For all database-related operations in your Supabase project (`SUPABASE_PROJECT_ID=uzqcjksjeoupwzkfhreo`).
- **repomix:** For advanced repo operations—summarization, packing/unpacking, code merges, analysis, and automated code manipulation.
- **github:** For all GitHub actions—issue and PR creation/updates, commenting, status checks, and automation of review processes.
- **git:** For local git operations—branching, commits, diffs, merges, reverts, logs, tagging, etc.
- **linkup, exa, tavily, firecrawl_scrape, firecrawl_crawl, firecrawl_extract, firecrawl_deep_research, context7, sequential-thinking:** For research, planning, up-to-date docs, codebase understanding, deep web lookups, stepwise reasoning, and generating code/architecture plans.
- **playwright:** For automated browser actions (integration/UI testing, web scraping/verification, automation of browser workflows).
- **time:** For time/date-related automation or simulation (e.g., logging, scheduled actions, test time manipulation).
- **google-maps:** For geo-location lookups, maps, routing, or related data (include only if relevant to the project).

**Always use the most appropriate tool for the task at hand—across research, planning, code implementation, automation, testing, or documentation. Invoke tools in parallel wherever possible for speed and coverage.**

$ARGUMENTS
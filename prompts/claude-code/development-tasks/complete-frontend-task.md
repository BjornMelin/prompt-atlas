## Complete Highest Priority Frontend Task

**Prioritize clear, maintainable, and efficient code and organization, delivering robust, fully featured, and best-practice solutions without unnecessary complexity. Solutions should be simple, yet powerful and comprehensive.**

1. Read `@tasks/TODO-FRONTEND.md` and select the highest-priority frontend task (just one main entry).
2. Review relevant official docs, community examples, and project documentation below. Reference project docs throughout and keep them updated.
3. Break down the selected frontend task into actionable subtasks using your built-in TODO tool. Actively manage and mark these as you work.
4. Use MCP server tools for research and implementation:
   - `firecrawl_scrape`: Scrape/extract from official docs and reference links.
   - `firecrawl_crawl`: Crawl doc sites for deeper or related content.
   - `firecrawl_deep_research`: For in-depth research on complex or broad topics.
   - `context7`: Fetch, read, and analyze API/library docs for examples/usage.
   - `exa`: For codebase exploration/static analysis.
   - `tavily`, `linkup`: For web search and community best practices if official docs lack detail.
   - `sequential-thinking`: For systematic reasoning or complex planning.
5. Plan and justify your approach for each subtask, based on research, best practices, and documentation.
6. Create a new branch (conventional-commits format). Implement the task, focusing on maintainability, clarity, and feature-completeness. Use Zod for schema validation.
7. Build or update the test suite for all new/changed frontend code. Ensure:
   - `npx biome lint --apply .` and `npx biome format --write .` both pass.
   - `npx vitest run` passes with ≥90% test coverage.
   - `npx playwright test` passes for all E2E scenarios.
8. Always run `npx biome lint --apply .` and `npx biome format --write .` before committing or submitting a PR. **Fix all linting/formatting issues before proceeding.**
9. Once all TODO tool subtasks are complete, update `@tasks/TODO-FRONTEND.md` to reflect completion, and add new/follow-up tasks if needed.
10. Update all relevant documentation, READMEs, and project docs to reflect changes, progress, and design decisions.
11. Commit and push changes. Open a PR via GitHub MCP server tools.
12. **STOP HERE** — Do not merge; use your PR review/merge command next.
13. **Final reminders:** Summarize any unresolved questions, ambiguities, or next steps; structure outputs logically with actionable details and referenced decisions; justify all major decisions with research and/or best practices; keep reference links handy for rapid doc lookups and optimal solutions.

---
### Reference Docs:
- React: https://react.dev/reference/react
- Next.js: https://nextjs.org/docs
- Tailwind CSS: https://tailwindcss.com/docs
- shadcn/ui: https://ui.shadcn.com/docs/installation
- TypeScript: https://www.typescriptlang.org/docs/
- Zod: https://zod.dev/
- Zustand: https://zustand.docs.pmnd.rs/getting-started/introduction
- TanStack Query: https://tanstack.com/query/latest/docs/react/overview
- React Hook Form: https://react-hook-form.com/get-started
- Vercel AI SDK: https://sdk.vercel.ai/docs
- Mapbox GL JS: https://docs.mapbox.com/mapbox-gl-js/api/
- Recharts: https://recharts.org/en-US/guide
- Chart.js: https://www.chartjs.org/docs/latest/
- Framer Motion: https://www.framer.com/motion/introduction/
- Vitest: https://vitest.dev/guide/
- React Testing Library: https://testing-library.com/docs/react-testing-library/intro
- Playwright: https://playwright.dev/docs/intro
- Sentry: https://docs.sentry.io/platforms/javascript/guides/nextjs/
- PostHog: https://posthog.com/docs/libraries/next-js
- OWASP: https://owasp.org/

$ARGUMENTS

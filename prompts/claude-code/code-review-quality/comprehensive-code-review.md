# Comprehensive Repository Code Review & Alignment

## Objective

Conduct a **complete, expert-level review** of the entire codebase and documentation, ensuring alignment with the latest architecture, best practices, and requirements in `@docs/REFACTOR/`, supporting documentation, completed GitHub issues, and outstanding tasks in `@TODO.md`.  
The review should result in actionable, prioritized recommendations and a clear, justified path to achieving a 10/10 score for all parts of the app.

---

## MCP Server Tool Usage Guide

- **pack_codebase:** Create codebase packs for logical, parallel review.
- **read_repomix_output:** Read/analyze each codebase pack's content.
- **context7:** Latest docs, code examples, and APIs.
- **firecrawl_scrape:** Scrape/extract docs or website content as needed.
- **firecrawl_crawl:** Crawl doc sites for broader or related content.
- **firecrawl_deep_research:** In-depth, multifaceted research/analysis.
- **exa:** Semantic search for docs, libraries, or code (primary).
- **tavily, linkup:** Additional research and doc exploration (secondary).
- **sequential-thinking:** Stepwise reasoning/planning for complex tasks.
- **git, github:** (Optional, context) Commits/PR analysis or diffing as needed.

---

## Step 1: Repository Structure Analysis & Packing Plan

1. **Scan and analyze the full repo structure.**
    - Review the directory tree, top-level and major subdirectories, and standalone critical files (configs, entrypoints, etc.).
    - Identify logical groupings for parallel review (by feature, service, architecture layer, etc.).
    - Note any legacy, deprecated, or potentially unused code/files for focused review/removal.

2. **Define and document the packing plan.**
    - Propose logical review packs, justify the rationale for each grouping, and flag areas needing extra scrutiny (e.g., legacy or heavily refactored).
    - Output the full packing plan to `docs/reviews/2025-05-30/packing-plan.md` before starting the detailed review.

---

## Step 2: Comprehensive Parallel Review Using Repomix Tools

For each codebase pack in the plan:
- Use **`pack_codebase`** to create the pack.
- Use **`read_repomix_output`** to read and analyze each pack in parallel.

**For every pack, conduct a thorough review covering:**
- Architecture & design patterns
- Code quality, maintainability, modularity
- Documentation completeness, clarity, accuracy
- Test coverage and reliability
- Alignment with all relevant docs (`@docs/REFACTOR/` and others), completed issues, and @TODO.md tasks

---

## Step 3: Research, Reasoning & Justification

- Use all available tools as needed for research and context (see tool guide above).
- For complex or ambiguous findings, use **`sequential-thinking`** to outline reasoning and alternative solutions.
- **Always justify major findings, scores, and recommendations** with research, best practices, explicit project documentation, or tool output/results.  
- Invite further discussion on tradeoffs or any complex recommendations.

---

## Step 4: Legacy, Obsolete, and Redundant Code Detection

- Proactively flag any files, code, or docs that are obsolete, redundant, or out-of-date after migrations/refactoring.
- Make clear, actionable recommendations for deletion, major update, or refactor.

---

## Step 5: Scoring, Assessment, and Actionable Recommendations

- For each component and documentation section, **score from 1–10** in:
    - Code quality & maintainability
    - Architecture & design
    - Documentation quality
    - Test coverage
    - System alignment/integration

- Be **completely honest and objective**; use expert judgment and avoid inflated scores.
- For every area, provide **detailed, actionable steps and suggestions** needed to reach a 10/10 score (including refactoring, tests, documentation, removal, or integrations as needed).

---

## Step 6: Output & Reporting

- **Do not write or modify any code—focus only on the review and action plan.**
- Save all results to: `docs/reviews/2025-05-30/`
    - For each review pack/section, create a markdown file with analysis, scores, and improvement plan.
    - Write the packing plan to `packing-plan.md`.
- At the end, output a comprehensive summary in `docs/reviews/2025-05-30/summary.md` including:
    - All scores for app and documentation components
    - Major findings, system-wide recommendations, and an overall prioritized checklist to achieve full alignment and modernization
    - Any files/directories clearly recommended for deletion or refactor
    - **Call out any system-wide issues, cross-cutting risks, or improvement opportunities that emerged from the review.**

---

## Review Guidelines

- Prioritize clarity, maintainability, and alignment with `@docs/REFACTOR/`.
- Pay close attention to outdated or unused files—recommend deletions where warranted.
- Justify all recommendations with best practices, research, and documentation references.
- Use parallel tool calls for speed and thoroughness.
- Be systematic, honest, and actionable in all scoring and suggestions.
- Provide constructive feedback and invite discussion on non-obvious tradeoffs.

---

**Begin only after documenting your packing plan and loading the full repository and documentation context.**

$ARGUMENTS
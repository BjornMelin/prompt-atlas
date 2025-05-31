## Finalize & Merge Branch

Prioritize clear, maintainable, and efficient code and organization, delivering robust, fully featured, and best-practice solutions without unnecessary complexity. Solutions should be simple, yet powerful and comprehensive.

1. Before starting, check for any remaining review subtasks in your built-in TODO tool. Confirm that all have been completed before proceeding.
2. Confirm all TODO files (`TODO.md`, and any project or module-specific TODO files) and all project documentation are updated to fully reflect all changes and work completed in the branch.
3. Ensure all automated checks, reviews, tests, and linters have passed.
4. Summarize any remaining open questions or future improvements in a final branch comment, issue note, or in project documentation for visibility to the next reviewer, developer, or future maintainer.
5. Merge the branch into the `main` branch via the approved workflow.
6. After merging:
   - Checkout `main` locally.
   - Run: `git pull`, `git fetch`, `git prune`.
   - Clean up merged feature branches both locally and remotely.
7. Communicate the successful merge and summarize changes to relevant team members if needed, either in a final branch comment, issue, or in team channels.

$ARGUMENTS
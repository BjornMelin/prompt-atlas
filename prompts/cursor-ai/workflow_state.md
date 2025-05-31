# Workflow State (STM + Rules + Log)

This file contains the dynamic state of the project workflow, including current phase, plan, rules, and action log. It is constantly updated during the development process.

## State

- Phase: ANALYZE | BLUEPRINT | CONSTRUCT | VALIDATE
- Status: READY | WORKING | BLOCKED | NEEDS_PLAN_APPROVAL | COMPLETED | FAILED
- CurrentItem: [Current item being processed, or null if not in iterative mode]

## Plan

[After completing the ANALYZE phase, the detailed plan will be written here. The plan should include step-by-step actions to implement the requested feature or solve the problem.]

1. [Step 1]
2. [Step 2]
3. [Step 3]
   ...

## Rules

### Global Rules

- Always operate based on the current Phase and Status in the State section
- Update the State section after completing each step or when status changes
- Record all actions, decisions, and observations in the Log section
- Use Sequential Thinking for complex problems, breaking them into manageable steps
- Follow coding standards and conventions defined in project_config.md
- Do not proceed to CONSTRUCT phase without user approval of the plan
- Clear context between processing different items to prevent context drift
- Update TokenizationResults after processing each item

### Phase-Specific Rules

#### ANALYZE Phase Rules

- Thoroughly understand all requirements before proceeding
- Research any unfamiliar concepts or technologies
- Ask clarifying questions if requirements are ambiguous
- Do not begin planning solutions until requirements are clear
- Identify potential challenges and dependencies
- Set State.Status = READY when analysis is complete

#### BLUEPRINT Phase Rules

- Create a detailed, step-by-step plan for implementation
- Include pseudocode where helpful
- Consider edge cases and error handling
- Break complex tasks into smaller subtasks
- Reference specific files and components from project_config.md
- Set State.Status = NEEDS_PLAN_APPROVAL when plan is complete
- Wait for user confirmation before proceeding to CONSTRUCT phase

#### CONSTRUCT Phase Rules

- Follow the approved plan precisely
- Implement one step at a time, testing each step
- Use appropriate Cursor tools (edit files, run commands)
- Handle errors according to strategy in project_config.md
- Update Log with results of each implementation step
- Set State.Status = BLOCKED if an unexpected obstacle is encountered
- Set State.Status = READY when implementation is complete

#### VALIDATE Phase Rules

- Test implementation against requirements
- Run appropriate validation tests (unit tests, linting, etc.)
- Fix any issues discovered during validation
- Document test results and any fixes made
- Set State.Status = COMPLETED when validation is successful
- Set State.Status = FAILED if validation cannot be completed

### Iteration Rules

- When processing items iteratively, track current item in State.CurrentItem
- Process one item at a time, completing full workflow for each
- After completing an item, store results in TokenizationResults
- Clear context before moving to next item to prevent "drift"
- Set State.CurrentItem = null when all items are processed

## Log

[This section contains a timestamped log of all actions, decisions, and observations made during the development process.]

YYYY-MM-DD HH:MM - [Action/Decision/Observation]
...

## Items

| Item ID | Text to Process   |
| ------- | ----------------- |
| item1   | [Text for item 1] |
| item2   | [Text for item 2] |
| ...     | ...               |

## TokenizationResults

| Item ID | Summary             | Token Count |
| ------- | ------------------- | ----------- |
| item1   | [Summary of item 1] | [Count]     |
| item2   | [Summary of item 2] | [Count]     |
| ...     | ...                 | ...         |

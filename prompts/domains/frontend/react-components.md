# React Component Development

## Description

This prompt helps you design and implement reusable, high-quality React components following best practices for modularity, performance, and accessibility.

## Use Cases

- Building UI component libraries
- Creating reusable application elements
- Implementing complex interactive components
- Converting design mockups to working components
- Refactoring existing component structures

## Parameters

- `[COMPONENT_TYPE]`: Type of component (button, form, card, etc.)
- `[FRAMEWORK]`: Framework context (Next.js, Create React App, Remix, etc.)
- `[STATE_MANAGEMENT]`: State management approach (hooks, context, Redux, etc.)
- `[STYLING_APPROACH]`: Styling methodology (CSS Modules, styled-components, Tailwind, etc.)
- `[ACCESSIBILITY_LEVEL]`: Accessibility requirements (WCAG AA, AAA, etc.)

## Example Usage

```markdown
I need to design a React component for:

1. Component Specifications:

   - Type: [COMPONENT_TYPE] (e.g., data table)
   - Framework: [FRAMEWORK] (e.g., Next.js 14)
   - Required features: [FEATURES] (e.g., sorting, pagination, filtering)
   - Styling approach: [STYLING_APPROACH] (e.g., Tailwind CSS)

2. Technical Requirements:

   - TypeScript type safety
   - State management: [STATE_MANAGEMENT] (e.g., React Query + local state)
   - Accessibility level: [ACCESSIBILITY_LEVEL] (e.g., WCAG 2.1 AA)
   - Browser compatibility: [BROWSER_SUPPORT] (e.g., modern browsers only)

3. Dependencies:

   - Available libraries: [LIBRARIES] (e.g., react-table, framer-motion)
   - Design system: [DESIGN_SYSTEM] (e.g., Material UI, Chakra)

4. Advanced Features (optional):
   - Animations: [ANIMATION_NEEDS] (e.g., smooth row transitions)
   - Performance optimizations: [PERF_REQUIREMENTS] (e.g., virtualization for large datasets)
   - Server integration: [SERVER_INTEGRATION] (e.g., GraphQL endpoints)

Focus area: [SPECIFIC_FUNCTIONALITY] (e.g., implementing column resizing)
```

## Expected Output

The AI assistant should provide:

1. Complete component implementation with TypeScript types
2. Proper state management and hooks usage
3. Event handling and user interaction patterns
4. Styling implementation
5. Accessibility considerations (ARIA attributes, keyboard navigation)
6. Usage examples
7. Props documentation

## Customization Guide

- For stateless components, you can simplify by removing state management requirements
- For design system integration, specify which components to extend or use
- Add specific performance requirements if the component will handle large datasets
- For form components, include validation requirements and error state handling
- Specify animation requirements if the component needs transitions or effects

## Version

- Current Version: 1.0
- Last Updated: 2025-05-07

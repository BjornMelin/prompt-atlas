# Component Architecture and Design Prompts

## Table of Contents
- [Component Design](#component-design)
- [Pattern Library](#pattern-library)
- [Component Testing](#component-testing)
- [State Management](#state-management)
- [Examples](#examples)

## Component Design

### Component Architecture
```markdown
Design component architecture for [application] with:
1. Design System Requirements:
   - Component hierarchy
   - Shared components
   - Component variants
   - Styling system

2. Technical Requirements:
   - Type safety
   - Accessibility
   - Responsiveness
   - Performance

3. Documentation:
   - Component API
   - Usage examples
   - Props interface
   - Storybook setup

4. Development Workflow:
   - Component creation
   - Review process
   - Testing strategy
   - Version control
```

### Component Library
```markdown
Create component library with:
1. Library Structure:
   - Core components
   - Composite components
   - Utility components
   - HOCs/Hooks

2. Technical Stack:
   - Build system
   - Type system
   - Styling solution
   - Documentation

3. Features:
   - Theming support
   - Accessibility
   - Internationalization
   - Responsive design

4. Distribution:
   - Package setup
   - Version management
   - Documentation
   - Example usage
```

## Pattern Library

### Design System
```markdown
Implement design system components:
1. Core Components:
   - Typography
   - Buttons
   - Forms
   - Layout

2. Component Features:
   - Variants
   - States
   - Animations
   - Composition

3. Technical Implementation:
   - Styling methodology
   - Props API
   - Event handling
   - Accessibility

4. Documentation:
   - Usage guidelines
   - Code examples
   - Best practices
   - Migration guides
```

## Component Testing

### Testing Strategy
```markdown
Design component testing strategy with:
1. Test Types:
   - Unit tests
   - Integration tests
   - Visual regression
   - Accessibility tests

2. Testing Setup:
   - Test framework
   - Test utilities
   - Mocking strategy
   - CI integration

3. Test Coverage:
   - Props validation
   - Event handling
   - State changes
   - Edge cases

4. Documentation:
   - Test examples
   - Coverage reports
   - Testing guidelines
   - Maintenance docs
```

## State Management

### Component State
```markdown
Design component state management for:
1. State Types:
   - Local state
   - Props
   - Context
   - External state

2. State Patterns:
   - Controlled components
   - Uncontrolled components
   - Compound components
   - Render props

3. Implementation:
   - State initialization
   - Update handlers
   - Side effects
   - Performance

4. Documentation:
   - State flow
   - Props API
   - Event handlers
   - Examples
```

## Examples

### Form Components
```markdown
Design form component system:
1. Components:
   - Input fields
   - Select dropdowns
   - Checkboxes/Radio
   - Form groups

2. Features:
   - Validation
   - Error handling
   - Accessibility
   - Responsive design

3. Implementation:
   - Form state
   - Field validation
   - Error messages
   - Submit handling

Focus: Form validation implementation
```

### Data Display Components
```markdown
Create data display components:
1. Components:
   - Tables
   - Lists
   - Cards
   - Grids

2. Features:
   - Sorting
   - Filtering
   - Pagination
   - Search

3. Implementation:
   - Data handling
   - State management
   - Event handling
   - Virtualization

Focus: Table component with sorting
```

## Best Practices

1. **Component Design**
   - Single responsibility
   - Composition over inheritance
   - Prop types/interfaces
   - Default props

2. **State Management**
   - Minimal state
   - Unidirectional data flow
   - Controlled vs uncontrolled
   - Performance optimization

3. **Testing**
   - Unit testing
   - Integration testing
   - Visual testing
   - Accessibility testing

4. **Documentation**
   - API documentation
   - Usage examples
   - Props documentation
   - Storybook stories

5. **Performance**
   - Memoization
   - Lazy loading
   - Event optimization
   - Render optimization

6. **Accessibility**
   - ARIA attributes
   - Keyboard navigation
   - Screen reader support
   - Color contrast

7. **Maintenance**
   - Version control
   - Change management
   - Deprecation strategy
   - Migration guides

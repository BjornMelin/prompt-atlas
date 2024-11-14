# React Development Prompts

## Table of Contents

- [Application Architecture](#application-architecture)
- [State Management](#state-management)
- [Routing and Navigation](#routing-and-navigation)
- [Testing Strategies](#testing-strategies)
- [Examples](#examples)

## Application Architecture

### Next.js Application

```markdown
I need to build a Next.js application for [use case] with:

1. Technical Requirements:

   - Next.js version: [13/14]
   - Rendering strategy: [SSR/SSG/ISR]
   - State management: [Redux/Zustand/Jotai]
   - Styling approach: [Tailwind/CSS Modules/styled-components]

2. Key Features:

   - Authentication system
   - Dynamic routing
   - API integration
   - SEO optimization

3. Performance Goals:

   - Core Web Vitals targets
   - Bundle size limits
   - Initial load time
   - Time to Interactive

4. Development Setup:
   - Project structure
   - Code organization
   - Build configuration
   - Development workflow

Current focus: [specific feature/component]
```

### React Application Structure

```markdown
Help structure a React application with:

1. Project Organization:

   - File structure
   - Component hierarchy
   - Module boundaries
   - Asset management

2. Technical Stack:

   - Build tools: [Vite/Create React App]
   - Type system: [TypeScript/PropTypes]
   - Testing framework
   - Linting/formatting

3. Architecture Patterns:

   - Component composition
   - Code splitting
   - Error boundaries
   - Performance optimization

4. Development Workflow:
   - Development setup
   - Build process
   - Deployment strategy
   - CI/CD integration
```

## State Management

### Application State

```markdown
Design state management for [application] using:

1. State Requirements:

   - Global state needs
   - Local state handling
   - Server state
   - Form state

2. Technical Approach:

   - State library: [Redux/Zustand/Context]
   - Data flow patterns
   - Side effect handling
   - Performance considerations

3. Implementation Details:

   - Store structure
   - Action patterns
   - Selector strategy
   - Middleware setup

4. Integration Points:
   - API integration
   - Local storage
   - Real-time updates
   - State persistence
```

## Routing and Navigation

### Route Structure

```markdown
Design routing system with:

1. Route Requirements:

   - Public routes
   - Protected routes
   - Nested routing
   - Dynamic routes

2. Navigation Features:

   - Deep linking
   - Breadcrumbs
   - Route guards
   - Loading states

3. Technical Implementation:

   - Router setup
   - Code splitting
   - State persistence
   - History management

4. SEO Considerations:
   - Meta tags
   - Structured data
   - Sitemap generation
   - Canonical URLs
```

## Testing Strategies

### Testing Implementation

```markdown
Design testing strategy for React application:

1. Testing Levels:

   - Unit tests
   - Integration tests
   - E2E tests
   - Performance tests

2. Testing Setup:

   - Test runner: [Jest/Vitest]
   - Testing library: [RTL/Enzyme]
   - E2E framework: [Cypress/Playwright]
   - CI integration

3. Test Coverage:

   - Component testing
   - Hook testing
   - State management
   - API integration

4. Best Practices:
   - Test organization
   - Mocking strategy
   - Snapshot testing
   - Performance testing
```

## Examples

### E-commerce Frontend

```markdown
Build e-commerce frontend with:

1. Features:

   - Product catalog
   - Shopping cart
   - Checkout flow
   - User accounts

2. Technical Stack:

   - Next.js 14
   - TypeScript
   - Tailwind CSS
   - React Query

3. Implementation:
   - Product listing
   - Cart management
   - Payment integration
   - Order tracking

Focus: Shopping cart implementation
```

### Dashboard Application

```markdown
Create admin dashboard with:

1. Features:

   - Data visualization
   - Real-time updates
   - CRUD operations
   - User management

2. Components:

   - Data grids
   - Charts/graphs
   - Forms
   - Navigation

3. Technical Stack:
   - React 18
   - Material-UI
   - React Query
   - Redux Toolkit

Focus: Data grid implementation
```

## Best Practices

1. **Component Design**

   - Single responsibility
   - Reusable components
   - Proper prop types
   - Error boundaries

2. **Performance**

   - Code splitting
   - Lazy loading
   - Memoization
   - Bundle optimization

3. **State Management**

   - Centralized store
   - Immutable updates
   - Selector patterns
   - Side effect handling

4. **Testing**

   - Component testing
   - Integration testing
   - Performance testing
   - Accessibility testing

5. **Development Workflow**

   - Code standards
   - Documentation
   - Review process
   - Deployment strategy

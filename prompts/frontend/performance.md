# Frontend Performance Optimization Prompts

## Table of Contents
- [Core Web Vitals](#core-web-vitals)
- [Bundle Optimization](#bundle-optimization)
- [Rendering Performance](#rendering-performance)
- [Resource Optimization](#resource-optimization)
- [Examples](#examples)

## Core Web Vitals

### Core Web Vitals Optimization
```markdown
Help optimize Core Web Vitals for [application] with:
1. Current Metrics:
   - LCP (Largest Contentful Paint): [time]
   - FID (First Input Delay): [time]
   - CLS (Cumulative Layout Shift): [score]
   - FCP (First Contentful Paint): [time]

2. Target Improvements:
   - LCP target: < 2.5s
   - FID target: < 100ms
   - CLS target: < 0.1
   - FCP target: < 1.8s

3. Implementation Areas:
   - Initial load optimization
   - Interaction responsiveness
   - Layout stability
   - Resource prioritization

4. Monitoring Setup:
   - Performance metrics
   - User monitoring
   - Lighthouse CI
   - Analytics integration
```

## Bundle Optimization

### Bundle Analysis
```markdown
Optimize application bundle with:
1. Current State:
   - Bundle size: [size]
   - Critical chunks
   - Dependencies
   - Load time

2. Optimization Targets:
   - Main bundle size
   - Code splitting
   - Tree shaking
   - Dynamic imports

3. Implementation Strategy:
   - Webpack/Vite config
   - Module federation
   - Dependency audit
   - Build optimization

4. Monitoring:
   - Bundle analysis
   - Performance budget
   - Size limits
   - Load metrics
```

## Rendering Performance

### React Rendering
```markdown
Optimize React rendering for:
1. Performance Issues:
   - Re-render frequency
   - Component complexity
   - State updates
   - Event handling

2. Optimization Methods:
   - Memoization
   - Virtual DOM
   - Lazy loading
   - Suspense usage

3. Implementation:
   - Component structure
   - Hook optimization
   - State management
   - Event handling

4. Measurement:
   - React DevTools
   - Performance profiler
   - Render tracking
   - Metrics collection
```

## Resource Optimization

### Asset Optimization
```markdown
Optimize frontend assets with:
1. Asset Types:
   - Images
   - Fonts
   - Scripts
   - Styles

2. Optimization Techniques:
   - Image optimization
   - Font loading
   - Script loading
   - CSS optimization

3. Delivery Strategy:
   - CDN usage
   - Caching policy
   - Preloading
   - Compression

4. Implementation:
   - Build process
   - Resource hints
   - Loading priorities
   - Error handling
```

## Examples

### E-commerce Performance
```markdown
Optimize e-commerce site performance:
1. Current Issues:
   - Slow product listing
   - Image loading
   - Cart updates
   - Checkout flow

2. Optimization Areas:
   - Image optimization
   - List virtualization
   - State management
   - API caching

3. Implementation:
   - Lazy loading
   - Progressive images
   - Request batching
   - Client caching

Focus: Product listing optimization
```

### Dashboard Performance
```markdown
Optimize dashboard performance:
1. Requirements:
   - Fast data loading
   - Real-time updates
   - Chart rendering
   - Filter operations

2. Optimization:
   - Data pagination
   - WebSocket efficiency
   - Chart optimization
   - Filter debouncing

3. Technical Approach:
   - Virtual scrolling
   - Data caching
   - Component optimization
   - Query management

Focus: Data grid performance
```

## Best Practices

1. **Loading Performance**
   - Route-based code splitting
   - Resource prioritization
   - Progressive loading
   - Caching strategy

2. **Runtime Performance**
   - Component optimization
   - State management
   - Event handling
   - Animation performance

3. **Rendering Performance**
   - Virtual DOM optimization
   - Render batching
   - Layout thrashing prevention
   - Paint optimization

4. **Asset Performance**
   - Image optimization
   - Font loading
   - Script loading
   - Style optimization

5. **Monitoring**
   - Performance metrics
   - User monitoring
   - Error tracking
   - Analytics

6. **Development Workflow**
   - Performance budgets
   - Automated testing
   - CI/CD integration
   - Documentation

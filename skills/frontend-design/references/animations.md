# CSS Animation Patterns

Collection of refined animation patterns for creating memorable micro-interactions.

## Basic Principles

### Timing Functions
```css
/* Custom easing functions */
--ease-smooth: cubic-bezier(0.25, 0.1, 0.25, 1);
--ease-bounce: cubic-bezier(0.68, -0.55, 0.265, 1.55);
--ease-elastic: cubic-bezier(0.175, 0.885, 0.32, 1.275);
```

### Duration Guidelines
```css
/* Animation durations */
--duration-fast: 150ms;
--duration-normal: 300ms;
--duration-slow: 500ms;
--duration-deliberate: 800ms;
```

## Common Patterns

### Hover Effects
```css
.btn-hover {
  transition: all var(--duration-normal) var(--ease-smooth);
  transform: translateY(0);
}

.btn-hover:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 25px rgba(0, 0, 0, 0.15);
}
```

### Loading Animations
```css
@keyframes pulse-subtle {
  0%, 100% { opacity: 1; }
  50% { opacity: 0.7; }
}

.loading-pulse {
  animation: pulse-subtle 2s var(--ease-smooth) infinite;
}
```

### Page Transitions
```css
.fade-in-up {
  animation: fadeInUp var(--duration-normal) var(--ease-smooth);
}

@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(30px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
```

### Micro-interactions
```css
/* Checkbox toggle */
.toggle-checkbox:checked + .toggle-slider {
  transform: translateX(20px);
  background: var(--color-success);
}

.toggle-slider {
  transition: all var(--duration-fast) var(--ease-smooth);
}
```

## Advanced Patterns

### Staggered Animations
```css
.stagger-item {
  animation: fadeInUp var(--duration-normal) var(--ease-smooth) forwards;
  opacity: 0;
}

.stagger-item:nth-child(1) { animation-delay: 0ms; }
.stagger-item:nth-child(2) { animation-delay: 100ms; }
.stagger-item:nth-child(3) { animation-delay: 200ms; }
```

### Morphing Shapes
```css
@keyframes morph {
  0% { border-radius: 60% 40% 30% 70%/60% 30% 70% 40%; }
  50% { border-radius: 30% 60% 70% 40%/50% 60% 30% 60%; }
  100% { border-radius: 60% 40% 30% 70%/60% 30% 70% 40%; }
}

.morph-shape {
  animation: morph 4s ease-in-out infinite;
}
```

### 3D Transformations
```css
.card-3d {
  transition: transform var(--duration-normal) var(--ease-smooth);
  transform-style: preserve-3d;
}

.card-3d:hover {
  transform: rotateY(10deg) rotateX(5deg) scale(1.02);
}
```

## Performance Tips

- Use `transform` and `opacity` for best performance
- Avoid animating `width`, `height`, `margin`, `padding`
- Use `will-change` for complex animations
- Consider `prefers-reduced-motion` for accessibility

## Accessibility

```css
@media (prefers-reduced-motion: reduce) {
  * {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
  }
}
```
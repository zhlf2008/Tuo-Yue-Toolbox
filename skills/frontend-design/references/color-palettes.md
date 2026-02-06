# Color Palettes

Curated color schemes for different aesthetic directions and contexts.

## Foundation Colors

### Neutral Palette
```css
:root {
  /* Grayscale */
  --gray-50: #fafafa;
  --gray-100: #f5f5f5;
  --gray-200: #e5e5e5;
  --gray-300: #d4d4d4;
  --gray-400: #a3a3a3;
  --gray-500: #737373;
  --gray-600: #525252;
  --gray-700: #404040;
  --gray-800: #262626;
  --gray-900: #171717;

  /* Semantic neutrals */
  --bg-primary: var(--gray-50);
  --bg-secondary: var(--gray-100);
  --border-light: var(--gray-200);
  --border-medium: var(--gray-300);
  --text-primary: var(--gray-900);
  --text-secondary: var(--gray-600);
  --text-muted: var(--gray-500);
}
```

## Theme Palettes

### Minimal/Elegant
```css
.minimal-theme {
  --primary: #2c5aa0;
  --primary-light: #4a76b8;
  --primary-dark: #1e3d72;
  --accent: #e8b4bc;
  --bg-primary: #fefefe;
  --bg-secondary: #f8f9fa;
  --text-primary: #2c2c2c;
  --text-secondary: #666;
}
```

### Warm/Organic
```css
.warm-theme {
  --primary: #e67e22;
  --primary-light: #f39c12;
  --primary-dark: #d35400;
  --accent: #27ae60;
  --bg-primary: #fef9f5;
  --bg-secondary: #fdebd0;
  --text-primary: #2c2c2c;
  --text-secondary: #7f8c8d;
}
```

### Luxury/Refined
```css
.luxury-theme {
  --primary: #8b7355;
  --primary-light: #a89276;
  --primary-dark: #6d5c46;
  --accent: #c9a96e;
  --bg-primary: #fcfaf8;
  --bg-secondary: #f8f6f3;
  --text-primary: #2c2c2c;
  --text-secondary: #666;
}
```

### Playful/Bright
```css
.playful-theme {
  --primary: #e74c3c;
  --primary-light: #ec7063;
  --primary-dark: #cb4335;
  --accent: #f39c12;
  --secondary: #3498db;
  --bg-primary: #fff;
  --bg-secondary: #f8f9fa;
  --text-primary: #2c3e50;
  --text-secondary: #7f8c8d;
}
```

### Dark/Industrial
```css
.dark-theme {
  --primary: #34495e;
  --primary-light: #4a6572;
  --primary-dark: #2c3e50;
  --accent: #e74c3c;
  --bg-primary: #1a1a1a;
  --bg-secondary: #2d2d2d;
  --text-primary: #ecf0f1;
  --text-secondary: #bdc3c7;
}
```

## Semantic Colors

### Status Colors
```css
:root {
  /* Success */
  --success-50: #f0f9f0;
  --success-100: #dcf2dc;
  --success-500: #27ae60;
  --success-700: #1e8449;

  /* Warning */
  --warning-50: #fef9e7;
  --warning-100: #fcf3cf;
  --warning-500: #f39c12;
  --warning-700: #b9770e;

  /* Error */
  --error-50: #fdf2f2;
  --error-100: #fadbd8;
  --error-500: #e74c3c;
  --error-700: #cb4335;

  /* Info */
  --info-50: #ebf5fb;
  --info-100: #d6eaf8;
  --info-500: #3498db;
  --info-700: #2874a6;
}
```

### Gradient Patterns
```css
.gradient-primary {
  background: linear-gradient(135deg, var(--primary), var(--primary-light));
}

.gradient-subtle {
  background: linear-gradient(135deg, 
    rgba(var(--primary-rgb), 0.1), 
    rgba(var(--primary-light-rgb), 0.05)
  );
}

.gradient-accent {
  background: linear-gradient(45deg, var(--accent), var(--primary));
}
```

## Usage Guidelines

### Color Contrast
- Ensure text contrast ratio of at least 4.5:1 for normal text
- Use 3:1 ratio for large text (18pt+ or 14pt+bold)
- Test colors with accessibility tools

### Color Psychology
- **Blue**: Trust, security, professionalism
- **Green**: Growth, success, nature
- **Orange**: Energy, creativity, warmth
- **Purple**: Luxury, creativity, wisdom
- **Red**: Urgency, passion, attention

### Implementation Tips
```css
/* Use CSS custom properties for theming */
:root {
  --primary-rgb: 44, 90, 160; /* Convert to RGB for opacity */
}

.background-with-opacity {
  background: rgba(var(--primary-rgb), 0.1);
}

/* Responsive color adjustments */
@media (prefers-color-scheme: dark) {
  :root {
    --bg-primary: #1a1a1a;
    --text-primary: #ffffff;
  }
}
```

## Testing Tools

- Use browser dev tools color contrast checker
- Test with color blindness simulators
- Validate with WebAIM contrast checker
- Consider using HSL color space for easier adjustments
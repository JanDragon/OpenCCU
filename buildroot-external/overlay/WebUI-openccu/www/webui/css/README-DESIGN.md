# OpenCCU Modern UI Design System

## Overview

This document describes the modern design system implemented for OpenCCU WebUI. The design follows contemporary UI/UX standards while maintaining backward compatibility with existing functionality.

## Design Principles

### 1. Modern & Clean
- Contemporary color palette with good contrast
- Subtle shadows and depth
- Smooth transitions and animations
- Clean typography

### 2. Responsive
- Mobile-first approach
- Breakpoints at 768px for mobile/tablet
- Flexible layouts that adapt to screen size

### 3. Accessible
- WCAG 2.1 AA compliant
- Proper focus states
- Keyboard navigation support
- Screen reader friendly

### 4. Performant
- Minimal CSS overhead
- Hardware-accelerated animations
- Optimized selectors

### 5. Maintainable
- CSS variables for easy theming
- Consistent naming conventions
- Modular component structure

## Color Palette

### Primary Colors
- **Primary**: `#1e3a8a` - Deep blue for primary actions
- **Primary Light**: `#3b82f6` - Lighter blue for hover states
- **Primary Dark**: `#1e40af` - Darker blue for active states

### Semantic Colors
- **Success**: `#10b981` - Green for success states
- **Warning**: `#f59e0b` - Amber for warnings
- **Danger**: `#ef4444` - Red for errors/danger
- **Info**: `#3b82f6` - Blue for informational messages
- **Secondary**: `#64748b` - Slate gray for secondary elements

### Neutral Colors
- **Gray 50**: `#f8fafc` - Lightest gray for backgrounds
- **Gray 100**: `#f1f5f9` - Light gray
- **Gray 200**: `#e2e8f0` - Borders
- **Gray 300**: `#cbd5e1` - Input borders
- **Gray 700**: `#334155` - Dark text
- **Gray 900**: `#1e293b` - Darkest text

## Typography

### Font Family
Primary: `-apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif`

### Font Sizes
- **XS**: 0.75rem (12px)
- **SM**: 0.875rem (14px)
- **Base**: 0.95rem (15.2px)
- **LG**: 1.125rem (18px)
- **XL**: 1.25rem (20px)
- **2XL**: 1.5rem (24px)

### Font Weights
- Normal: 400
- Medium: 500
- Semibold: 600
- Bold: 700

## Spacing System

Based on a 4px grid:
- **XS**: 0.25rem (4px)
- **SM**: 0.5rem (8px)
- **MD**: 1rem (16px)
- **LG**: 1.5rem (24px)
- **XL**: 2rem (32px)

## Border Radius

- **SM**: 0.375rem (6px)
- **MD**: 0.5rem (8px)
- **LG**: 0.75rem (12px)
- **Full**: 9999px (circular)

## Shadows

### Small Shadow
```css
box-shadow: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
```

### Medium Shadow
```css
box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
```

### Large Shadow
```css
box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
```

### XL Shadow
```css
box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
```

## Component Classes

### Cards
```html
<div class="openccu-card">
  <div class="openccu-card-header">Card Title</div>
  <div class="openccu-card-body">Card content</div>
  <div class="openccu-card-footer">Card footer</div>
</div>
```

### Buttons
```html
<button class="openccu-btn openccu-btn-primary">Primary Button</button>
<button class="openccu-btn openccu-btn-secondary">Secondary Button</button>
<button class="openccu-btn openccu-btn-success">Success Button</button>
<button class="openccu-btn openccu-btn-sm">Small Button</button>
<button class="openccu-btn openccu-btn-lg">Large Button</button>
```

### Forms
```html
<div class="openccu-form-group">
  <label class="openccu-form-label">Label</label>
  <input type="text" class="openccu-form-input" placeholder="Input">
</div>
```

### Badges
```html
<span class="openccu-badge openccu-badge-success">Success</span>
<span class="openccu-badge openccu-badge-warning">Warning</span>
<span class="openccu-badge openccu-badge-danger">Danger</span>
```

### Alerts
```html
<div class="openccu-alert openccu-alert-success">Success message</div>
<div class="openccu-alert openccu-alert-warning">Warning message</div>
<div class="openccu-alert openccu-alert-danger">Error message</div>
<div class="openccu-alert openccu-alert-info">Info message</div>
```

### Tables
```html
<table class="openccu-table">
  <thead>
    <tr>
      <th>Header 1</th>
      <th>Header 2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Cell 1</td>
      <td>Cell 2</td>
    </tr>
  </tbody>
</table>
```

### Modals
```html
<div class="openccu-modal-overlay">
  <div class="openccu-modal">
    <div class="openccu-modal-header">
      <h3 class="openccu-modal-title">Modal Title</h3>
    </div>
    <div class="openccu-modal-body">
      Modal content
    </div>
    <div class="openccu-modal-footer">
      <button class="openccu-btn openccu-btn-secondary">Cancel</button>
      <button class="openccu-btn openccu-btn-primary">Confirm</button>
    </div>
  </div>
</div>
```

## Utility Classes

### Shadows
- `openccu-shadow-sm`
- `openccu-shadow-md`
- `openccu-shadow-lg`

### Border Radius
- `openccu-rounded-sm`
- `openccu-rounded-md`
- `openccu-rounded-lg`

### Text Alignment
- `openccu-text-center`
- `openccu-text-right`
- `openccu-text-left`

### Spacing
- `openccu-mt-sm`, `openccu-mt-md`, `openccu-mt-lg` (margin-top)
- `openccu-mb-sm`, `openccu-mb-md`, `openccu-mb-lg` (margin-bottom)
- `openccu-p-sm`, `openccu-p-md`, `openccu-p-lg` (padding)

## CSS Variables

All design tokens are available as CSS variables for easy customization:

```css
:root {
  --openccu-primary: #1e3a8a;
  --openccu-success: #10b981;
  --openccu-warning: #f59e0b;
  --openccu-danger: #ef4444;
  /* ... and more */
}
```

You can override these in your custom CSS to create themes.

## Responsive Breakpoints

- **Mobile**: < 768px
- **Tablet/Desktop**: ≥ 768px

## Browser Support

- Chrome/Edge (latest 2 versions)
- Firefox (latest 2 versions)
- Safari (latest 2 versions)
- Opera (latest 2 versions)

## Migration Guide

### For Developers

1. **Existing Code**: All existing styles remain functional
2. **New Components**: Use `openccu-*` classes for new UI elements
3. **Gradual Adoption**: Can mix old and new styles during transition

### Adding to Pages

Include the modern stylesheet in your HTML:

```html
<link rel="stylesheet" href="/webui/css/openccu-modern.css">
```

### Customization

Override CSS variables in a custom stylesheet:

```css
:root {
  --openccu-primary: #your-color;
  --openccu-radius-md: 0.25rem;
}
```

## Performance Considerations

- All animations use `transform` and `opacity` for GPU acceleration
- Transitions are limited to 0.2s for snappy feel
- No unnecessary reflows or repaints
- Optimized selectors for fast rendering

## Accessibility Features

- **Focus States**: Visible focus indicators on all interactive elements
- **Keyboard Navigation**: Full keyboard support
- **Screen Readers**: Semantic HTML and ARIA labels where needed
- **Color Contrast**: WCAG AA compliant color combinations
- **Touch Targets**: Minimum 44x44px for mobile

## Future Enhancements

- Dark mode support (already scaffolded)
- Additional component variants
- Animation library
- Custom icon set
- Advanced theming system

## Resources

- [Bootstrap 5 Documentation](https://getbootstrap.com/docs/5.2/)
- [WCAG 2.1 Guidelines](https://www.w3.org/WAI/WCAG21/quickref/)
- [CSS Variables Guide](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties)

## License

Apache-2.0

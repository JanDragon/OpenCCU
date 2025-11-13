# OpenCCU Modern UI - Quick Reference Guide

## Quick Start

### 1. Include the CSS

```html
<link rel="stylesheet" href="/webui/css/extern/main.min.css">
<link rel="stylesheet" href="/webui/css/extern/hmBootstrap.css">
<link rel="stylesheet" href="/webui/css/openccu-modern.css">
```

### 2. Add the Modern Class (Optional)

```html
<body class="openccu-modern">
  <!-- Your content -->
</body>
```

## Cheat Sheet

### Colors

| Variable | Value | Use Case |
|----------|-------|----------|
| `--openccu-primary` | #1e3a8a | Primary actions, headers |
| `--openccu-success` | #10b981 | Success states, confirmations |
| `--openccu-warning` | #f59e0b | Warnings, cautions |
| `--openccu-danger` | #ef4444 | Errors, deletions |
| `--openccu-info` | #3b82f6 | Information, highlights |
| `--openccu-secondary` | #64748b | Secondary actions |

### Buttons

```html
<!-- Primary Button -->
<button class="openccu-btn openccu-btn-primary">Primary</button>

<!-- Secondary Button -->
<button class="openccu-btn openccu-btn-secondary">Secondary</button>

<!-- Success Button -->
<button class="openccu-btn openccu-btn-success">Success</button>

<!-- Warning Button -->
<button class="openccu-btn openccu-btn-warning">Warning</button>

<!-- Danger Button -->
<button class="openccu-btn openccu-btn-danger">Danger</button>

<!-- Small Button -->
<button class="openccu-btn openccu-btn-primary openccu-btn-sm">Small</button>

<!-- Large Button -->
<button class="openccu-btn openccu-btn-primary openccu-btn-lg">Large</button>
```

### Cards

```html
<div class="openccu-card">
  <div class="openccu-card-header">Card Title</div>
  <div class="openccu-card-body">
    <p>Card content goes here</p>
  </div>
  <div class="openccu-card-footer">
    <button class="openccu-btn openccu-btn-primary">Action</button>
  </div>
</div>
```

### Forms

```html
<!-- Text Input -->
<div class="openccu-form-group">
  <label class="openccu-form-label">Label</label>
  <input type="text" class="openccu-form-input" placeholder="Enter text">
</div>

<!-- Select -->
<div class="openccu-form-group">
  <label class="openccu-form-label">Select Option</label>
  <select class="openccu-form-select">
    <option>Option 1</option>
    <option>Option 2</option>
  </select>
</div>

<!-- Textarea -->
<div class="openccu-form-group">
  <label class="openccu-form-label">Description</label>
  <textarea class="openccu-form-textarea" rows="3"></textarea>
</div>
```

### Badges

```html
<span class="openccu-badge openccu-badge-primary">Primary</span>
<span class="openccu-badge openccu-badge-success">Success</span>
<span class="openccu-badge openccu-badge-warning">Warning</span>
<span class="openccu-badge openccu-badge-danger">Danger</span>
<span class="openccu-badge openccu-badge-secondary">Secondary</span>
```

### Alerts

```html
<!-- Success Alert -->
<div class="openccu-alert openccu-alert-success">
  <strong>Success!</strong> Operation completed successfully.
</div>

<!-- Info Alert -->
<div class="openccu-alert openccu-alert-info">
  <strong>Info:</strong> Important information.
</div>

<!-- Warning Alert -->
<div class="openccu-alert openccu-alert-warning">
  <strong>Warning!</strong> Please be careful.
</div>

<!-- Danger Alert -->
<div class="openccu-alert openccu-alert-danger">
  <strong>Error!</strong> Something went wrong.
</div>
```

### Tables

```html
<table class="openccu-table">
  <thead>
    <tr>
      <th>Column 1</th>
      <th>Column 2</th>
      <th>Column 3</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Data 1</td>
      <td>Data 2</td>
      <td>Data 3</td>
    </tr>
  </tbody>
</table>
```

### Tabs

```html
<div class="openccu-tabs">
  <button class="openccu-tab active">Tab 1</button>
  <button class="openccu-tab">Tab 2</button>
  <button class="openccu-tab">Tab 3</button>
</div>
```

### Modal

```html
<div class="openccu-modal-overlay">
  <div class="openccu-modal">
    <div class="openccu-modal-header">
      <h3 class="openccu-modal-title">Modal Title</h3>
    </div>
    <div class="openccu-modal-body">
      <p>Modal content</p>
    </div>
    <div class="openccu-modal-footer">
      <button class="openccu-btn openccu-btn-secondary">Cancel</button>
      <button class="openccu-btn openccu-btn-primary">Confirm</button>
    </div>
  </div>
</div>
```

### Loading States

```html
<!-- Spinner -->
<div class="openccu-loading"></div>

<!-- Skeleton -->
<div class="openccu-skeleton" style="height: 20px; width: 100%;"></div>
```

## Utility Classes

### Shadows

```html
<div class="openccu-shadow-sm">Small shadow</div>
<div class="openccu-shadow-md">Medium shadow</div>
<div class="openccu-shadow-lg">Large shadow</div>
```

### Border Radius

```html
<div class="openccu-rounded-sm">Small radius</div>
<div class="openccu-rounded-md">Medium radius</div>
<div class="openccu-rounded-lg">Large radius</div>
```

### Text Alignment

```html
<div class="openccu-text-left">Left aligned</div>
<div class="openccu-text-center">Center aligned</div>
<div class="openccu-text-right">Right aligned</div>
```

### Spacing

```html
<!-- Margin Top -->
<div class="openccu-mt-sm">Small margin top</div>
<div class="openccu-mt-md">Medium margin top</div>
<div class="openccu-mt-lg">Large margin top</div>

<!-- Margin Bottom -->
<div class="openccu-mb-sm">Small margin bottom</div>
<div class="openccu-mb-md">Medium margin bottom</div>
<div class="openccu-mb-lg">Large margin bottom</div>

<!-- Padding -->
<div class="openccu-p-sm">Small padding</div>
<div class="openccu-p-md">Medium padding</div>
<div class="openccu-p-lg">Large padding</div>
```

## Responsive Design

### Breakpoints

- **Mobile**: < 768px
- **Desktop**: ≥ 768px

### Media Query Example

```css
/* Mobile styles */
.my-element {
  padding: 0.5rem;
}

/* Desktop styles */
@media (min-width: 768px) {
  .my-element {
    padding: 1rem;
  }
}
```

## Customization

### Override CSS Variables

```css
:root {
  --openccu-primary: #your-color;
  --openccu-spacing-md: 1.5rem;
  --openccu-radius-md: 0.75rem;
}
```

### Custom Theme

```css
/* custom-theme.css */
:root {
  /* Colors */
  --openccu-primary: #2563eb;
  --openccu-success: #059669;
  
  /* Spacing */
  --openccu-spacing-md: 1.25rem;
  
  /* Typography */
  --openccu-font-size-base: 1rem;
  
  /* Borders */
  --openccu-radius-md: 0.75rem;
}
```

## Common Patterns

### Form with Submit Button

```html
<form>
  <div class="openccu-form-group">
    <label class="openccu-form-label">Username</label>
    <input type="text" class="openccu-form-input" required>
  </div>
  
  <div class="openccu-form-group">
    <label class="openccu-form-label">Password</label>
    <input type="password" class="openccu-form-input" required>
  </div>
  
  <button type="submit" class="openccu-btn openccu-btn-primary">
    Login
  </button>
</form>
```

### Status Indicator

```html
<div class="openccu-card">
  <div class="openccu-card-header">System Status</div>
  <div class="openccu-card-body">
    <p>
      Status: 
      <span class="openccu-badge openccu-badge-success">Online</span>
    </p>
    <p>
      Devices: 
      <span class="openccu-badge openccu-badge-primary">12</span>
    </p>
  </div>
</div>
```

### Action List

```html
<div class="openccu-card">
  <div class="openccu-card-header">Actions</div>
  <div class="openccu-card-body">
    <button class="openccu-btn openccu-btn-success openccu-mb-sm">
      Start
    </button>
    <button class="openccu-btn openccu-btn-warning openccu-mb-sm">
      Pause
    </button>
    <button class="openccu-btn openccu-btn-danger">
      Stop
    </button>
  </div>
</div>
```

### Data Table with Actions

```html
<table class="openccu-table">
  <thead>
    <tr>
      <th>Name</th>
      <th>Status</th>
      <th>Actions</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Device 1</td>
      <td>
        <span class="openccu-badge openccu-badge-success">Online</span>
      </td>
      <td>
        <button class="openccu-btn openccu-btn-primary openccu-btn-sm">
          Edit
        </button>
      </td>
    </tr>
  </tbody>
</table>
```

## Tips & Best Practices

### 1. Use Semantic Colors
- Green (success) for positive actions
- Red (danger) for destructive actions
- Yellow (warning) for cautions
- Blue (info/primary) for neutral actions

### 2. Consistent Spacing
- Use spacing utilities instead of custom margins
- Stick to the defined spacing scale

### 3. Responsive Design
- Test on mobile devices
- Use relative units (rem, %)
- Consider touch targets

### 4. Accessibility
- Always include labels for inputs
- Use semantic HTML
- Test keyboard navigation
- Check color contrast

### 5. Performance
- Use CSS classes instead of inline styles
- Avoid deep nesting
- Leverage CSS variables

## Troubleshooting

### Styles Not Applying

1. Check CSS is included in correct order
2. Verify class names are correct
3. Check for conflicting styles
4. Clear browser cache

### Button Not Showing

```html
<!-- Wrong -->
<button class="openccu-btn">Click Me</button>

<!-- Correct (need variant) -->
<button class="openccu-btn openccu-btn-primary">Click Me</button>
```

### Form Input Too Wide

```html
<!-- Add a container -->
<div style="max-width: 500px;">
  <div class="openccu-form-group">
    <input type="text" class="openccu-form-input">
  </div>
</div>
```

## Resources

- **Full Documentation**: [UI-REDESIGN.md](./UI-REDESIGN.md)
- **Design System**: [README-DESIGN.md](../buildroot-external/overlay/WebUI-openccu/www/webui/css/README-DESIGN.md)
- **Demo Page**: http://openccu/webui/design-demo.html
- **Before/After**: [UI-BEFORE-AFTER.md](./UI-BEFORE-AFTER.md)

## Support

For issues or questions:
1. Check the documentation
2. View the demo page
3. Search existing issues
4. Open a new issue if needed

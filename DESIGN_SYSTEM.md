# Convopia - Design System

## Typography
- **Font Sans**: Geist
- **Font Serif**: Geist
- **Font Mono**: Geist

## Dark Mode Colors

### Primary Colors
- **Primary**: `#c0a080`
- **Primary Foreground**: `#2d2621`

### Secondary Colors
- **Secondary**: `#4a4039`
- **Secondary Foreground**: `#ece5d8`

### Accent Colors
- **Accent**: `#59493e`
- **Accent Foreground**: `#ece5d8`

### Background & Surface
- **Background**: `#2d2621`
- **Foreground**: `#ece5d8`
- **Card**: `#3a322c`
- **Card Foreground**: `#ece5d8`
- **Popover**: `#3a322c`
- **Popover Foreground**: `#ece5d8`

### UI Elements
- **Border**: `#4a4039`
- **Input**: `#4a4039`
- **Ring**: `#c0a080`

### States
- **Muted**: `#3a322c`
- **Muted Foreground**: `#c5b0ac`
- **Destructive**: `#b54a35`
- **Destructive Foreground**: `#ffffff`

### Sidebar
- **Sidebar**: `#2d2621`
- **Sidebar Foreground**: `#ece5d8`
- **Sidebar Primary**: `#c0a080`
- **Sidebar Primary Foreground**: `#2d2621`
- **Sidebar Accent**: `#59493e`
- **Sidebar Accent Foreground**: `#ece5d8`
- **Sidebar Border**: `#4a4039`
- **Sidebar Ring**: `#c0a080`

### Charts
- **Chart 1**: `#c0a080`
- **Chart 2**: `#b3906f`
- **Chart 3**: `#a67c52`
- **Chart 4**: `#8d6e4c`
- **Chart 5**: `#735a3a`

---

## Light Mode Colors

### Primary Colors
- **Primary**: `#a67c52`
- **Primary Foreground**: `#ffffff`

### Secondary Colors
- **Secondary**: `#e2d8c3`
- **Secondary Foreground**: `#5c4d3f`

### Accent Colors
- **Accent**: `#d4c8aa`
- **Accent Foreground**: `#4a3f35`

### Background & Surface
- **Background**: `#f5f1e6`
- **Foreground**: `#4a3f35`
- **Card**: `#fffcf5`
- **Card Foreground**: `#4a3f35`
- **Popover**: `#fffcf5`
- **Popover Foreground**: `#4a3f35`

### UI Elements
- **Border**: `#dbd0ba`
- **Input**: `#dbd0ba`
- **Ring**: `#a67c52`

### States
- **Muted**: `#ece5d8`
- **Muted Foreground**: `#7d6b56`
- **Destructive**: `#b54a35`
- **Destructive Foreground**: `#ffffff`

### Sidebar
- **Sidebar**: `#ece5d8`
- **Sidebar Foreground**: `#4a3f35`
- **Sidebar Primary**: `#a67c52`
- **Sidebar Primary Foreground**: `#ffffff`
- **Sidebar Accent**: `#d4c8aa`
- **Sidebar Accent Foreground**: `#4a3f35`
- **Sidebar Border**: `#dbd0ba`
- **Sidebar Ring**: `#a67c52`

### Charts
- **Chart 1**: `#a67c52`
- **Chart 2**: `#8d6e4c`
- **Chart 3**: `#735a3a`
- **Chart 4**: `#b3906f`
- **Chart 5**: `#c0a080`

---

## Other Design Tokens

### Border Radius
- **Radius**: `0.125rem` (2px)

### Shadows
- **X Offset**: `0px`
- **Y Offset**: `0px`
- **Blur**: `0px`
- **Spread**: `0px`
- **Color**: `#0000000d` (black with 5% opacity)

---

## Implementation Notes

### Tailwind CSS Configuration
These colors should be added to `tailwind.config.ts` under the `theme.extend.colors` section with CSS variables:

```typescript
colors: {
  border: "hsl(var(--border))",
  input: "hsl(var(--input))",
  ring: "hsl(var(--ring))",
  background: "hsl(var(--background))",
  foreground: "hsl(var(--foreground))",
  primary: {
    DEFAULT: "hsl(var(--primary))",
    foreground: "hsl(var(--primary-foreground))",
  },
  // ... etc
}
```

### CSS Variables (globals.css)
```css
@layer base {
  :root {
    --background: 43 20% 95%;
    --foreground: 30 14% 26%;
    --primary: 30 35% 49%;
    --primary-foreground: 0 0% 100%;
    /* ... etc */
  }

  .dark {
    --background: 24 14% 16%;
    --foreground: 30 25% 91%;
    --primary: 30 31% 63%;
    --primary-foreground: 24 14% 16%;
    /* ... etc */
  }
}
```

### shadcn/ui Integration
This color scheme is compatible with shadcn/ui's theming system. Use `npx shadcn@latest init` and configure with these custom colors.

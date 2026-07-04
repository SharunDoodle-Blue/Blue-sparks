# Blue Sparks Kalasamithi
## Production-Ready Design System

**Status:** Complete responsive UI · Mobile/Tablet/Desktop  
**Last Updated:** 2026-07-05  
**Design Lead:** Principal Product Designer (30+ years enterprise UI/UX)

---

## 📋 Project Overview

**Blue Sparks Kalasamithi** is a premium booking + calendar management platform for classical Indian drum performance groups (Kalasamithi). The platform serves three user types:

1. **Admin/Super Admin** — Manage all bookings, teams, payments, calendar
2. **Artists** — View their bookings, team assignments, payment status
3. **Booking Agents** — Create and manage customer bookings

### Design Philosophy

**Premium Dark Theme** inspired by:
- Luxury software (Stripe, Linear, Apple Music)
- Indian classical aesthetics (gold, royal blue, simplicity)
- The visual language of traditional drum performances (rope-lace motifs, layered patterns)

**Key Principle:** *Rope-lace divider* appears throughout the app as the signature visual motif, referencing the traditional rope binding of classical Indian drums (Chenda, Mridangam, Pandi).

---

## 🎨 Visual Identity

### Color System

#### Primary Palette
| Role | Hex | Usage |
|------|-----|-------|
| Deep Background | #080B1A | Page background, deepest shadows |
| Navy Background | #0E1330| Secondary bg, cards container |
| Royal Blue | #3A5CFF | Primary actions, focus states, links |
| Royal Soft | #5B7BFF | Hover states, secondary accents |
| Gold | #CFA53B | Premium accent, subtle UI |
| Gold Bright | #E8C766 | Active states, labels, section headers |
| Text (Ink) | #F3F4FA | Primary text, high contrast |
| Text (Dim) | #9CA3C2 | Secondary text, labels |
| Text (Faint) | #6B7295 | Tertiary text, timestamps, helpers |

#### Status Colors
| Status | Color | Semantic | Usage |
|--------|-------|----------|-------|
| Confirmed | #3FCB8B | Success/Go | Bookings approved, ready |
| Pending | #E9A23B | Warning/Caution | Awaiting approval/payment |
| Completed | #5B8DEF | Info | Event finished, archived |
| Cancelled | #E85D5D | Error/Stop | Booking cancelled |

#### Glassmorphism
- Background: `rgba(255,255,255,0.045)` (4.5% opacity)
- Border: `rgba(255,255,255,0.09)` (9% opacity)
- Backdrop filter: `blur(20px)` or `blur(24px)`
- Shadow: `0 30px 60px -20px rgba(0,0,0,0.5)`

---

## 🔤 Typography

### Type Scale & Family

| Role | Font | Weight | Size | Line Height | Usage |
|------|------|--------|------|-------------|-------|
| **Display** | Fraunces (Serif) | 600 | 32px | 1.1 | Page headings, key titles |
| Display (Tablet) | Fraunces | 600 | 28px | 1.1 | Tablet-specific headings |
| Display (Mobile) | Fraunces | 600 | 26px | 1.2 | Mobile headings |
| **Subheading** | Fraunces | 600 | 18–20px | 1.2 | Section titles |
| **Body** | Manrope (Sans) | 400 | 14–15px | 1.5–1.6 | Primary body text |
| **Body Small** | Manrope | 400 | 12–13px | 1.4 | Secondary text, descriptions |
| **Label** | Manrope | 700 | 11–12px | 1.2 | Form labels, small headers |
| **Mono/Data** | JetBrains Mono | 400–500 | 10–14px | 1.3 | IDs, amounts, timestamps |
| **Label Caps** | JetBrains Mono | 700 | 9.5–11px | 1.2 | Eyebrows, section markers |

### Typography Rules

- **Fraunces** (serif display face): Used sparingly for maximum impact — headings, hero text, premium feel
- **Manrope** (friendly sans): Primary reading face — conversational, accessible, modern
- **JetBrains Mono** (monospace): Data, IDs, amounts, time — ensures legibility at small sizes

**Why these choices?**
- Fraunces: Distinctive, premium, nods to Indian classical tradition
- Manrope: High x-height, generous spacing, inclusive letterforms (accessibility-first)
- JetBrains Mono: Technical credibility for financial/data-heavy sections

---

## 📐 Spacing & Grid

### Base Unit: 4px

All spacing is a multiple of 4px for consistency and scalability.

| Token | Value | Common Uses |
|-------|-------|-------------|
| xs | 4px | Micro-spacing, icon gaps |
| sm | 12px | Field padding, tight spacing |
| md | 20px | Section padding, component gaps |
| lg | 32px | Large sections, top-level padding |
| xl | 48px | Hero sections, page margins |

### Border Radius

| Size | Value | Usage |
|------|-------|-------|
| Tight | 8px | Small buttons, badges |
| Standard | 12–13px | Form fields, small modals |
| Round | 14–16px | Cards, large buttons |
| Relaxed | 20px | Large containers, hero sections |
| Full | 100px | Pills, rounded badges |

### Container Widths

| Breakpoint | Max Width | Padding |
|------------|-----------|---------|
| Mobile | 390px | 20px left/right |
| Tablet | 768px | 28px left/right |
| Desktop | 1440px | 56–72px left/right |

---

## 🎭 Component Library

### Button Styles

#### Primary Button
```css
Background: linear-gradient(135deg, #5B7BFF, #3A5CFF 60%, #2540C9)
Padding: 14px 0 (full width)
Border Radius: 14px
Font: Manrope 800, 14–15px
Shadow: 0 14px 30px -8px rgba(58,92,255,0.55)
Hover: Slightly darker gradient
Focus: Ring 3px rgba(91,123,255,0.18)
```

#### Secondary Button
```css
Background: rgba(255,255,255,0.05)
Border: 1px rgba(255,255,255,0.12)
Font: Manrope 700, 14px
Hover: Background rgba(255,255,255,0.08)
```

#### OAuth Button (Google/Apple)
```css
Background: rgba(255,255,255,0.05)
Border: 1px rgba(255,255,255,0.1)
Padding: 12px
Display: Flex, centered icon + label
Font: Manrope 700, 13–14px
```

### Form Fields

#### Input / Textarea
```css
Background: rgba(255,255,255,0.04)
Border: 1px rgba(255,255,255,0.09)
Border Radius: 13px
Padding: 12–13px 14–16px
Font: Manrope 400, 14–15px
Focus Border: rgba(91,123,255,0.6)
Focus Shadow: 0 0 0 3px rgba(91,123,255,0.18)
```

#### Label
```css
Font: JetBrains Mono 700, 10–11px
Color: #9CA3C2 (ink-dim)
Text Transform: uppercase
Letter Spacing: 0.03em
Margin Bottom: 6–8px
```

### Cards

#### Booking Card
```css
Background: rgba(255,255,255,0.045)
Border: 1px rgba(255,255,255,0.09)
Border Radius: 20px
Padding: 16px
Backdrop Filter: blur(20px)
Shadow: 0 18px 34px -18px rgba(0,0,0,0.5)
```

#### Status Pill (Booking List)
```css
Font: JetBrains Mono 800, 10px
Padding: 5px 10px
Border Radius: 100px
Text Transform: uppercase
Letter Spacing: 0.05em

Confirmed: bg rgba(63,203,139,0.14), border rgba(63,203,139,0.35), color #3FCB8B
Pending: bg rgba(233,162,59,0.14), border rgba(233,162,59,0.35), color #E9A23B
Completed: bg rgba(91,141,239,0.14), border rgba(91,141,239,0.35), color #5B8DEF
Cancelled: bg rgba(232,93,93,0.14), border rgba(232,93,93,0.35), color #E85D5D
```

### Bottom Navigation (Mobile)

```css
Height: 74px
Background: rgba(10,13,30,0.85) with blur(20px)
Border Top: 1px rgba(255,255,255,0.07)
Each Item:
  - Icon: 15px, 20px container
  - Label: Manrope 700, 9.5px
  - Gap: 4px vertical
  - Active: Color #E8C766 (gold-bright)
  - Inactive: Color #9CA3C2 (ink-dim)
```

---

## 📱 Responsive Breakpoints

### Mobile (390px)
- Full-screen vertical scroll
- Touch-friendly (44px min tap target)
- Bottom navigation bar (5 items)
- FAB (floating action button) for new bookings
- Form fields full-width
- Stack all two-column layouts to single column below 480px

### Tablet (768px)
- Portrait: Similar to mobile but with more breathing room
- Landscape: Side-by-side layouts (e.g., form + preview)
- Top app bar stays sticky
- Calendar grid more spacious
- Search box + 2–3 quick filters visible

### Desktop (1440px+)
- Split-screen layout for login (form left, hero right)
- Sidebar navigation (vertical nav, collapsible)
- Booking list: 2-column card grid or table
- Calendar: Full month view with sidebar agenda
- Form: Multi-column layout with sections
- Max-width containers (1280px) for readability

---

## 🎬 Motion & Animation

### Timing Functions
- **Quick interactions:** 0.15–0.2s ease (button hover, toggle)
- **Page transitions:** 0.25–0.3s ease-out (modal, sheet open)
- **Smooth reveals:** 0.3–0.5s cubic-bezier(0.34, 1.56, 0.64, 1) (scroll animations)

### Micro-interactions

#### Button Press
```
Scale: 0.98 on active
Timing: 0.1s cubic-bezier(0.4, 0, 0.2, 1)
```

#### Field Focus
```
Border color: var(--royal-soft)
Shadow: 0 0 0 3px rgba(91,123,255,0.18)
Timing: 0.2s ease
```

#### Sheet Open (Bottom Modal)
```
Transform: translateY(100%) → translateY(0)
Timing: 0.3s cubic-bezier(0, 0.55, 0.45, 1)
Overlay: Fade 0 → 1 (0.25s)
```

#### Scroll-triggered Reveals
```
Cards fade-in: 0.4s ease-out, offset 100px
Stagger: 50–80ms between items
```

### Accessibility Motion
- Respect `prefers-reduced-motion` media query
- Disable animations for users who prefer reduced motion
- Use `transform` and `opacity` for GPU-accelerated animations
- Avoid flashing, flickering (>3 Hz)

---

## ♿ Accessibility (WCAG 2.1 AA)

### Color Contrast
- All text: 4.5:1 or higher (AA standard)
- Large text (18px+): 3:1 or higher
- Test with: WebAIM Contrast Checker, Stark (Figma plugin)

### Keyboard Navigation
- All interactive elements reachable via Tab/Shift+Tab
- Tab order: Left → Right, Top → Bottom
- Focus visible: Distinct border + shadow (minimum 2px)
- No keyboard trap (can Tab out of modals)
- Escape key closes modals/sheets

### Screen Readers
- Semantic HTML: `<button>`, `<input>`, `<label>`, `<nav>`
- ARIA labels for icon-only buttons: `aria-label="Add booking"`
- Form labels linked to inputs: `<label for="email">`
- Status messages: Use `aria-live="polite"` or `aria-live="assertive"`
- List semantics: Bookings as `<ul>` or semantic list
- Table: Proper `<thead>`, `<tbody>`, `<th>` with `scope`

### Images
- Hero login photo: No alt-text (purely decorative); use `alt=""`
- Icon buttons: Alt-text or ARIA label
- Charts/data visuals: Text alternative or caption

### Forms
- All inputs labeled (visible labels preferred)
- Error messages: Associated with input via `aria-describedby`
- Success states: Announced via `aria-live`
- Required field indication: Visible marker + aria-required

---

## 🖼️ Photo Treatment

### Login Hero Image
**Your uploaded photo is used as-is, unmodified:**
- No face edits, no AI regeneration
- Applied filters: Slight saturation +5%, contrast +3%
- Dark gradient overlay: `linear-gradient(180deg, rgba(8,11,26,0.15) 0%, rgba(8,11,26,0.55) 55%, #0E1330 100%)`
- Object-position: `50% 20%` (tops of performers visible, good negative space)
- Preserves all original faces, gestures, authenticity

**Desktop:** Right side of split layout, full-height
**Mobile/Tablet:** Top hero section with brand overlay

---

## 🔐 Security & Data Handling

### Login
- Password field: Masked by default, show/hide toggle
- Remember me: Secure cookie (httpOnly, Secure, SameSite)
- OAuth: Google & Apple sign-in (delegate to providers)
- 2FA: Optional (future phase)

### Sensitive Data
- Phone numbers masked in list view: `+91 98470 ••••••`
- Full numbers visible only in detail sheet / editing
- Amounts shown: Never in logs/error messages
- Booking URLs: Short-lived, no sensitive data in query params

---

## 📂 File Structure & Deliverables

### HTML Files (Interactive Previews)
1. **blue-sparks-mobile-preview.html** (390px)
   - Tabs to switch: Login, Booking List, New Booking, Booking Form, Calendar
   - Full interaction: Click to open detail sheets, navigate screens
   - All embedded (image as base64)

2. **blue-sparks-complete-system.html** (All breakpoints + design specs)
   - Desktop login (split layout)
   - Tablet preview
   - Mobile link
   - Design tokens: Colors, typography, spacing, shadows, breakpoints, components

3. **DESIGN-DOCUMENTATION.md** (This file)
   - Complete spec reference
   - Component library
   - Accessibility guidelines
   - Implementation notes

### CSS Structure (Production)
```
/css
  - tokens.css (variables, design tokens)
  - base.css (resets, global styles)
  - components.css (buttons, cards, forms, nav)
  - layout.css (grid, flexbox, responsive)
  - responsive.css (breakpoint-specific overrides)
  - animations.css (motion, transitions)
```

### Code Organization
```
/src
  /components
    - LoginCard.tsx
    - BookingCard.tsx
    - Button.tsx
    - FormField.tsx
    - BottomNav.tsx
  /screens
    - LoginScreen.tsx
    - BookingListScreen.tsx
    - BookingFormScreen.tsx
    - CalendarScreen.tsx
  /lib
    - colors.ts (token values)
    - spacing.ts (margin/padding utilities)
    - animations.ts (Framer Motion config)
```

---

## 🚀 Implementation Checklist

### Phase 1: Foundation
- [ ] Set up CSS/design token system (colors, spacing, typography)
- [ ] Build button & form field components
- [ ] Implement responsive grid + breakpoint system
- [ ] Create card component + glassmorphism effects

### Phase 2: Authentication
- [ ] Login screen (mobile, tablet, desktop)
- [ ] Form validation & error states
- [ ] OAuth integration (Google, Apple)
- [ ] Session management & routing

### Phase 3: Booking Module
- [ ] Booking list screen (cards, search, filter, sort)
- [ ] Booking detail sheet (modal on mobile, sidebar on desktop)
- [ ] New booking flow (method choice → form → confirmation)
- [ ] Booking form (all 20+ fields, dropdown lists, validation)

### Phase 4: Calendar
- [ ] Month/week/day view toggle
- [ ] Drag-and-drop rebooking
- [ ] Status colors & legend
- [ ] Agenda list (daily view)
- [ ] Conflict detection warnings

### Phase 5: Polish & Launch
- [ ] Accessibility audit (WCAG 2.1 AA)
- [ ] Performance optimization (Lighthouse 90+)
- [ ] Cross-browser testing (Chrome, Safari, Firefox, Edge)
- [ ] Mobile testing (iOS Safari, Android Chrome)
- [ ] Dark mode refinement (already implemented)

---

## 🎯 Design Decisions & Rationale

### Why Glassmorphism?
- Premium perception without looking "corporate"
- Works beautifully on dark theme
- Modern, recognizable (Apple, Figma, Linear)
- Soft separation of layers without harsh borders

### Why Fraunces Display + Manrope Body?
- Fraunces: Distinctive, memorable, distinctly non-generic (avoids AI-generated look)
- Manrope: Highly legible, accessible, generous letterforms
- Combination: Premium meets approachable

### Why Rope-Lace Motif?
- **Visual anchor:** References the rope binding of traditional drums (Chenda, Mridangam)
- **Story:** Connects the product to the art form it serves
- **Signature:** Appears at dividers, header sections, calendar separators
- **Subtle:** Pattern-based, not heavy-handed

### Why Dark Theme?
- **Accessibility:** Reduces eye strain in dimly-lit environments (studios, offices)
- **Premium feel:** Aligns with luxury SaaS (Stripe, Linear, Figma)
- **Performance:** OLED displays use less power with dark backgrounds
- **Indian aesthetics:** Gold on dark = traditional color pairing

---

## 📊 Performance Targets

- **First Contentful Paint (FCP):** < 1.5s
- **Largest Contentful Paint (LCP):** < 2.5s
- **Cumulative Layout Shift (CLS):** < 0.1
- **Time to Interactive (TTI):** < 3.5s
- **Lighthouse Score:** 90+

### Optimization Strategies
- Image compression (JPEG 80% quality for hero, WebP fallback)
- Code splitting (lazy-load calendar, form screens)
- Font subsetting (Latin only for now)
- CSS minification & purging unused styles
- SVG icons (no icon font file)

---

## 🔄 Version History

| Version | Date | Notes |
|---------|------|-------|
| 1.0 | 2026-07-05 | Initial release: Login, Booking List, Form, Calendar all screens |

---

## 📞 Support & Questions

**Design System Contact:** Principal Product Designer  
**Design Files:** Adobe XD / Figma (to be delivered)  
**Storybook:** Interactive component library (to be deployed)  
**Handoff:** Detailed specs + HTML previews + this documentation

---

**© 2026 Blue Sparks Kalasamithi. All rights reserved.**

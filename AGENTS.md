# RS Chinese Fast Food - Agent Guidelines

## 📱 CORE DIRECTIVE: MOBILE-FIRST DESIGN (STRICT PRIORITY)

> **CRITICAL REQUIREMENT:**
> This website is built primarily for **mobile smartphone users** (95%+ of traffic comes via mobile devices through WhatsApp links, QR code scans at tables, Google Maps, and local social media).
>
> **Every feature, UI change, layout modification, and enhancement MUST be designed, tested, and optimized for mobile screens first (360px - 430px viewport widths).**

---

### Key Mobile-First Principles to Always Follow:

1. **Touch Targets & Thumb Zone:**
   - Buttons, quantity counters (+ / -), category pills, and links must have a minimum touch target of **44px × 44px** with comfortable padding.
   - Key interactive elements (Cart checkout button, search, category navigation) must be easily reachable with one thumb.

2. **No iOS Auto-Zoom on Form Inputs:**
   - All `<input>`, `<textarea>`, and `<select>` elements must have a font size of at least `16px` to prevent Safari on iOS from automatically zooming the viewport when focused.

3. **Horizontal Scroll & Responsive Viewport Safety:**
   - Maintain zero horizontal layout overflow (`overflow-x: hidden` safety on body/container).
   - Category navigation pills and filter chips must support smooth, frictionless horizontal swipe (`overflow-x: auto; -webkit-overflow-scrolling: touch; scrollbar-width: none;`).

4. **Cart Modal & Bottom Sheets:**
   - On mobile screens, the cart modal operates as an ergonomic bottom sheet or full-height slide-over with sticky action buttons at the bottom.
   - Floating cart bar must always stay anchored at the bottom without blocking critical content.

5. **Performance on 2G / 3G / 4G Cellular Networks:**
   - Optimize and compress all images (`loading="lazy"` on menu items).
   - Lightweight zero-framework vanilla HTML/CSS/JS for instant First Contentful Paint (< 1 second).
   - Preserve offline and asset caching via Service Worker (`sw.js`) and PWA manifest (`manifest.json`).

6. **Desktop View as Progressive Enhancement:**
   - Desktop view is a centered, cleanly contained max-width layout (or dual-column view) that progressively enhances the mobile experience without breaking mobile styling.

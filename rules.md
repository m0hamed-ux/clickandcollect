## UI rules:
🎯 Purpose

This document defines the design rules, principles, and constraints that the AI agent must follow when generating website UI components, layouts, and visual systems to ensure high usability, visual appeal, and optimal user experience.

📐 1. GENERAL DESIGN PHILOSOPHY

Design must be user-centric, prioritizing clarity, accessibility, and usability.

Follow established design systems (e.g., Material Design, Apple HIG, Fluent) unless otherwise specified.

Design must serve the content, not vice versa.

Every UI element must serve a purpose — no visual noise.

🖥️ 2. LAYOUT & STRUCTURE
✅ DO:

Use a 12-column grid system for responsive layouts.

Maintain consistent spacing (use a scale: 4px, 8px, 16px, 24px, 32px, 64px).

Use clear content hierarchy:

H1 for page title

H2-H4 for sub-sections

Use consistent font sizes, weights, and spacing

Apply visual grouping to related elements (cards, modals, sections).

❌ AVOID:

Overlapping elements unless explicitly styled (e.g., parallax)

Excessive horizontal scrolling

Poor contrast or overly busy layouts

🎨 3. COLOR & THEME
✅ DO:

Use a cohesive color palette: primary, secondary, accent, background, text.

Ensure WCAG AA/AAA contrast ratio compliance for readability.

Support dark mode and light mode where applicable.

Use neutral backgrounds to let content stand out.

❌ AVOID:

Clashing colors

Overuse of gradients or shadows

Redundant color usage (colors must have functional meaning)

🔠 4. TYPOGRAPHY
✅ DO:

Use scalable and accessible fonts (e.g., Inter, Roboto, SF Pro, Open Sans).

Set line height to 1.4–1.6 for readability.

Use max 2 font families across the UI.

Maintain clear heading hierarchy and logical content flow.

❌ AVOID:

Fonts smaller than 14px for body content

More than 3 font weights

Using novelty fonts unless contextually appropriate (e.g., branding sites)

🧭 5. NAVIGATION
✅ DO:

Ensure navigation is intuitive, consistent, and visible.

Use sticky headers or sidebars when needed.

Highlight the current page/state clearly.

Ensure mobile-friendly menus (hamburger, collapsible, etc.).

❌ AVOID:

Deeply nested menu items (over 3 levels)

Invisible navbars (unless contextual)

Unlabeled icons without tooltips or text

📱 6. RESPONSIVE DESIGN
✅ DO:

Follow mobile-first design principles.

Use media queries for breakpoints (e.g., 480px, 768px, 1024px, 1440px).

Ensure all tap targets are at least 48x48px.

Design components to adapt fluidly to screen sizes.

❌ AVOID:

Fixed-width layouts

Hidden content on smaller screens (use collapsible)

Horizontal scroll (unless intentionally part of the experience)

🧩 7. COMPONENT DESIGN
✅ DO:

Use reusable components: buttons, cards, inputs, modals, tabs, etc.

Maintain consistent component states:

Default

Hover

Active

Disabled

Loading

Add accessible labels and ARIA roles as needed.

Use icons sparingly and meaningfully.

❌ AVOID:

Inconsistent paddings/margins between components

Mixing multiple styles of buttons or inputs

Redundant tooltips or labels

🔁 8. INTERACTIONS & ANIMATIONS
✅ DO:

Use animations to enhance feedback and guide user behavior.

Transitions should be:

< 300ms for UI responsiveness

Easing: use ease-in-out, ease-out

Animate on:

Button clicks

Modal transitions

Hover/focus states

❌ AVOID:

Excessive or distracting animations

Animations that block interactions

Inconsistent animation timing

♿ 9. ACCESSIBILITY (A11Y)
✅ DO:

Follow WCAG 2.1 compliance

Ensure keyboard navigation for all interactive components

Provide alt text for all images

Use semantic HTML structure: <header>, <main>, <footer>, <nav>, etc.

❌ AVOID:

Color-only indicators (use icons or labels as well)

Non-descriptive link text ("Click here")

Unlabeled form inputs

📊 10. UX WRITING & CONTENT
✅ DO:

Use concise, action-oriented language

Maintain a consistent tone: Friendly, professional, or brand-specific

Use microcopy to clarify intent (e.g., button labels, error states)

Provide feedback on actions (e.g., form submitted, error message)

❌ AVOID:

Technical jargon for general audiences

Vague button labels (e.g., “Submit” instead of “Send Message”)

Overloading the user with choices or information

🧠 11. USER FLOW & JOURNEY
✅ DO:

Design for clear user goals (e.g., sign-up, purchase, learn).

Use progress indicators for multi-step flows.

Include confirmation states (e.g., “Your order has been placed”).

Ensure no dead ends — provide next steps (e.g., CTA buttons).

❌ AVOID:

Requiring registration before value is shown

Breaking user expectations (e.g., back button behavior)

Dead-end pages without navigation or CTA

🔐 12. FORMS & INPUT UX
✅ DO:

Group related inputs with clear labels

Validate inputs in real-time (client-side)

Use descriptive error messages

Autofocus and autocomplete where appropriate

❌ AVOID:

Long, unsegmented forms

Using placeholders as labels

Showing errors only after submission

⚙️ 13. PERFORMANCE & LOAD EXPERIENCE
✅ DO:

Optimize images and use modern formats (e.g., WebP)

Lazy load below-the-fold content

Use skeleton loaders or spinners for async content

Minimize layout shifts (CLS)

❌ AVOID:

Blocking assets (e.g., slow scripts in <head>)

Excessive external requests

Full-page reloads for SPA interactions

🧪 14. TESTABILITY

Generated UIs must be testable with automated tools:

Semantic HTML

Test-friendly attributes (e.g., data-testid)

Accessible roles for elements
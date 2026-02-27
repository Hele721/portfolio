# plan3 — Header & navigation (site structure + accessibility)

## Context
The portfolio includes a fixed header with site title and navigation to sections (⁠ #main ⁠, ⁠ #projects ⁠, ⁠ #contact ⁠). This feature is essential for UX and also helps meet accessibility expectations (clear landmark, nav label, skip link).

## Phase 1 — Planning (AI-assisted)
### Prompt
I need to implement a semantic header/navigation for a one-page scrollytelling portfolio.
Constraints:
•⁠  ⁠Use semantic elements (⁠ <header> ⁠, ⁠ <nav> ⁠).
•⁠  ⁠Provide a skip link to main content.
•⁠  ⁠Navigation should link to in-page anchors: About, Projects, Contact.
•⁠  ⁠Mobile-friendly (simple list is OK; no JS required).
•⁠  ⁠Ensure good accessibility: ⁠ aria-label ⁠, focus states, clear text.
Please provide a plan and HTML structure. Include optional CSS ideas (sticky header, spacing).

### AI Plan / Response (summarized)
1.⁠ ⁠Add a skip link as the first focusable element (⁠ <a class="skip-link" href="#main"> ⁠).
2.⁠ ⁠Create ⁠ <header role="banner"> ⁠ with:
   - Site title (⁠ h1 ⁠ or styled element).
   - ⁠ <nav aria-label="Principal"> ⁠ containing a simple ⁠ <ul><li><a> ⁠ list.
3.⁠ ⁠Ensure the target anchors exist (⁠ id="main" ⁠, ⁠ id="projects" ⁠, ⁠ id="contact" ⁠).
4.⁠ ⁠Add CSS:
   - Keep header readable and consistent with typography.
   - Add hover/focus states for links.
   - Optional sticky positioning if desired, ensuring it does not cover anchors (use scroll-margin on sections).

## Phase 2 — Implementation
### What I implemented
•⁠  ⁠Added skip link to jump directly to ⁠ <main id="main"> ⁠.
•⁠  ⁠Implemented semantic header and navigation with anchor links to:
  - ⁠ #main ⁠ (Sobre mí)
  - ⁠ #projects ⁠ (Proyectos)
  - ⁠ #contact ⁠ (Contacto)
•⁠  ⁠Ensured headings/IDs are present in the corresponding sections.
•⁠  ⁠Added/kept basic CSS for focus/hover visibility and spacing.

### Files changed
•⁠  ⁠⁠ index.html ⁠
•⁠  ⁠⁠ assets/css/_accessibility.css ⁠ (skip link / focus styles)
•⁠  ⁠⁠ assets/css/_layout.css ⁠ or ⁠ _components.css ⁠ (header layout)

### Notes / Validation
•⁠  ⁠Tested keyboard navigation:
  - Tab shows skip link.
  - Nav links are reachable and visible on focus.
•⁠  ⁠Confirmed anchors scroll to the intended sections.
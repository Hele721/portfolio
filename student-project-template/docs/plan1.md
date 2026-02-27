# plan1 — Custom 404 page (GitHub Pages)

## Context
This project is deployed on GitHub Pages. When users navigate to a non-existing route, GitHub Pages serves a 404 page. The assignment requires a custom ⁠ 404.html ⁠ at repository root to provide a better user experience and (optionally) redirect users back to the homepage.

## Phase 1 — Planning (AI-assisted)
### Prompt
I need to add a ⁠ 404.html ⁠ page for a static portfolio deployed on GitHub Pages.  
Constraints:
•⁠  ⁠File must be in repository root.
•⁠  ⁠Should provide a minimal message and a link back to ⁠ index.html ⁠.
•⁠  ⁠Preferably auto-redirect after a short delay.
•⁠  ⁠Must be accessible (language set, clear heading, readable text).
Please provide a short implementation plan and a minimal HTML template.

### AI Plan / Response (summarized)
1.⁠ ⁠Create ⁠ 404.html ⁠ in repository root so GitHub Pages serves it automatically.
2.⁠ ⁠Include:
   - ⁠ <meta charset="UTF-8"> ⁠, viewport, and a descriptive ⁠ <title> ⁠.
   - Clear message (⁠ <h1>404</h1> ⁠) + short explanation.
   - A link back to ⁠ index.html ⁠.
3.⁠ ⁠Add an auto-redirect:
   - Use ⁠ meta http-equiv="refresh" ⁠ for a simple redirect after 1–3 seconds.
   - Add a JS fallback ⁠ window.location.replace("./index.html") ⁠ in case refresh is blocked.
4.⁠ ⁠Keep styles minimal (inline) to avoid asset loading issues on 404 routes.

## Phase 2 — Implementation
### What I implemented
•⁠  ⁠Added ⁠ 404.html ⁠ at repository root.
•⁠  ⁠Implemented:
  - Basic HTML structure (lang, meta tags, title).
  - ⁠ h1 ⁠ + explanatory text.
  - Link to homepage.
  - Auto-redirect via meta refresh + JS fallback.

### Files changed
•⁠  ⁠⁠ 404.html ⁠ (new)

### Notes / Validation
•⁠  ⁠Verified that navigating to a non-existent route serves ⁠ 404.html ⁠ on GitHub Pages.
•⁠  ⁠Verified that the “Back to home” link works and redirect triggers.
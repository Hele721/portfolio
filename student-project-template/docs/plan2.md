# plan2 — Footer (required deliverable + repository link)

## Context
The assignment requires a footer. The portfolio already includes a final CTA section, but a proper ⁠ <footer> ⁠ is needed for compliance and to provide attribution/copyright and a link to the repository.

## Phase 1 — Planning (AI-assisted)
### Prompt
I need to add a footer to a single-page portfolio (⁠ index.html ⁠).  
Constraints:
•⁠  ⁠Must be semantic (⁠ <footer> ⁠).
•⁠  ⁠Should include copyright and a link to the GitHub repository.
•⁠  ⁠Should match existing typography and spacing.
•⁠  ⁠Keep it simple and responsive.
Please propose a brief plan and the exact HTML + minimal CSS to add.

### AI Plan / Response (summarized)
1.⁠ ⁠Add ⁠ <footer> ⁠ after ⁠ </main> ⁠ and before closing ⁠ </body> ⁠.
2.⁠ ⁠Content:
   - Copyright line with name and year.
   - Link to GitHub repo (opens in new tab with ⁠ rel="noopener noreferrer" ⁠).
3.⁠ ⁠CSS:
   - Center text.
   - Use spacing tokens and existing font variables.
   - Underline link for clarity and accessibility.
4.⁠ ⁠Keep footer small so it does not compete with the final CTA.

## Phase 2 — Implementation
### What I implemented
•⁠  ⁠Added a semantic ⁠ <footer class="site-footer"> ⁠ at the end of the page.
•⁠  ⁠Included:
  - Copyright.
  - Link to the repository.
•⁠  ⁠Styled footer with simple alignment and spacing consistent with the design system.

### Files changed
•⁠  ⁠⁠ index.html ⁠
•⁠  ⁠⁠ assets/css/... ⁠ (where footer styles live; e.g., ⁠ _components.css ⁠ or ⁠ _layout.css ⁠)

### Notes / Validation
•⁠  ⁠Verified footer appears on desktop and mobile.
•⁠  ⁠Verified link opens correctly and is readable with keyboard navigation.
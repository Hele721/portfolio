# plan4 — Design system tweaks (space + color adjustments)

## Context
During implementation, some spacing and color decisions needed refinement so the portfolio looked consistent. The project uses CSS variables/tokens (e.g., colors, spacing scale) and component styles. Small adjustments were required to align typography, contrast, and layout rhythm.

## Phase 1 — Planning (AI-assisted)
### Prompt
I want to refine spacing and color consistency in my static portfolio.
Constraints:
•⁠  ⁠Use CSS variables (design tokens) for color and spacing whenever possible.
•⁠  ⁠Keep a limited palette (primary/accent + neutrals).
•⁠  ⁠Ensure readable contrast for text.
•⁠  ⁠Avoid random one-off margins; prefer token-based spacing (⁠ --space-sm ⁠, ⁠ --space-md ⁠, etc.).
Please provide a short plan for how to approach these refinements and what to check.

### AI Plan / Response (summarized)
1.⁠ ⁠Audit tokens:
   - Define/confirm primary color, neutrals, and text colors in ⁠ _variables.css ⁠.
   - Confirm spacing scale is consistent and referenced by components/layout.
2.⁠ ⁠Replace one-off spacing with token usage:
   - Use ⁠ margin/padding ⁠ with ⁠ --space-* ⁠ variables.
3.⁠ ⁠Check contrast/readability:
   - Ensure headings and body text have sufficient contrast against backgrounds.
4.⁠ ⁠Validate in responsive:
   - Ensure spacing scales down on small screens.
5.⁠ ⁠Keep changes minimal and consistent:
   - Prefer small adjustments in tokens over many local overrides.

## Phase 2 — Implementation
### What I implemented
•⁠  ⁠Adjusted color/spacing using CSS variables instead of hardcoded values where possible.
•⁠  ⁠Applied small layout rhythm tweaks (padding/margins) to improve readability and consistency.
•⁠  ⁠Updated a few component styles to align with the token scale.

### Files changed
•⁠  ⁠⁠ assets/css/_variables.css ⁠
•⁠  ⁠⁠ assets/css/_layout.css ⁠
•⁠  ⁠⁠ assets/css/_components.css ⁠
•⁠  ⁠(Optional) ⁠ assets/css/_responsive.css ⁠ if mobile spacing needed adjustments

### Notes / Validation
•⁠  ⁠Checked main sections visually for consistent vertical rhythm.
•⁠  ⁠Confirmed text remains readable on hero/cards and in the parallax section.
•⁠  ⁠Confirmed changes do not break scrollytelling animations or layout on mobile.
# CLAUDE.md

## Project

Single-page interactive tool showing how Oak Park property taxes are allocated across Village departments. Self-contained `index.html` with embedded CSS and JS, hosted via GitHub Pages.

## Repository

- **Owner:** Cory J. Wesley, Oak Park Village Trustee
- **Website:** corywesley.com
- **Repo:** cjwesley/OakParkBudgetBreakdown

## Workflow

- Always create a PR immediately after pushing a feature branch — do not wait to be asked.
- After creating a PR, ask the user if they'd like it merged.
- Keep commits focused and descriptive.

## Technical Notes

- `index.html` is fully self-contained — no external CSS, JS, or assets.
- CSS variables are defined in `:root` within a `<style>` block; all dynamic elements use inline styles with CSS class hooks for responsive media queries.
- The JS `refresh()` function rebuilds the bar chart on every interaction — any new CSS classes must be assigned inside `refresh()`.
- Responsive breakpoints: 600px (mobile), 380px (extra small).
- Budget data is based on the Village of Oak Park FY2026 adopted budget.

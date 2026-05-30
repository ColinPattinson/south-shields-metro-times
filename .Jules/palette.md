## 2025-05-14 - Accessible Color Contrast for Transit Status
**Learning:** Standard UI blues (#3498db) and greens (#27ae60) often fail WCAG AA contrast ratios (4.5:1) against white text. Switching to #206694 and #1b7a43 maintains semantic meaning while ensuring accessibility.
**Action:** Use WCAG AA compliant color palettes for all state-indicating backgrounds.

## 2025-05-14 - Screen Reader Context for Color-Coded States
**Learning:** Purely visual state indicators (like background colors) are invisible to screen readers. Using the "Screen Reader Context Pattern" (a .sr-only span that updates text alongside visual changes) ensures parity of information.
**Action:** Pair every semantic color change with a corresponding update to an aria-live region or .sr-only label.

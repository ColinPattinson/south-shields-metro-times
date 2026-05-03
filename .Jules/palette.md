## 2026-05-03 - Screen Reader Context Pattern
**Learning:** Purely color-coded state transitions (like blue for scheduled vs green for live) are invisible to screen readers and color-blind users. Using a visually hidden utility class to update text labels in sync with color changes provides essential context without cluttering the visual UI.
**Action:** Always include a hidden status span when using color to indicate state, and update its text content whenever the color changes.

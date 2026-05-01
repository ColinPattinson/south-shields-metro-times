## 2025-05-12 - Screen Reader Context Pattern
**Learning:** For dynamic UI components that change background color to signify state (e.g., Live vs. Scheduled), visual users get immediate feedback, but screen reader users miss this. Using a visually hidden `sr-only` span that updates its text alongside the visual change provides the necessary context.
**Action:** Always pair visual state changes with a screen-reader-only text update or appropriate ARIA attributes.

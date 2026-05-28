## 2025-05-15 - Screen Reader Context Pattern
**Learning:** Purely visual indicators (like background colors for 'Live' vs 'Scheduled' status) are invisible to assistive technologies. Using a visually hidden element (.sr-only) that updates its text alongside visual changes ensures screen reader users receive the same state information.
**Action:** Always pair visual-only state changes with a hidden text description and use aria-live="polite" on the container to announce updates.

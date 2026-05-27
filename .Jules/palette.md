## 2026-05-27 - Screen Reader Context Pattern
**Learning:** Visual-only state changes (like color shifts for 'Live' vs 'Scheduled' data) are invisible to screen readers. Using a visually hidden element (.sr-only) that updates its text within an aria-live region ensures all users receive state updates.
**Action:** Implement a .sr-only class and pair visual indicators with hidden descriptive text labels that update dynamically.

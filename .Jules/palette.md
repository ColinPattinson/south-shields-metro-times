## 2026-06-20 - Accessible Status Indicators
**Learning:** Visual-only status indicators (like background colors or dots) are inaccessible to screen reader and color-blind users. Combining them with visually hidden (`.sr-only`) text labels and `aria-live` ensures that all users receive the same state information.
**Action:** Always pair color-coded states with an `.sr-only` description and use `aria-live="polite"` for dynamic updates to these states.

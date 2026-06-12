## 2025-05-14 - Screen Reader Context Pattern
**Learning:** Visual-only indicators (like color-coded backgrounds or status dots) are inaccessible to screen reader users unless accompanied by visually hidden text that provides the same context.
**Action:** Use a `.sr-only` class to provide descriptive labels (e.g., "Live prediction:") alongside dynamic visual updates, and ensure status indicators are marked with `aria-hidden="true"` when redundant.

## 2025-05-14 - Inclusive Scheduling Logic
**Learning:** Filtering schedules using strict inequality (e.g., `m > currentMinute`) creates a "dead zone" where departures occurring within the current minute are hidden from the user.
**Action:** Use inclusive checks (e.g., `m >= currentMinute`) and implement a "Due now" state for zero-minute countdowns to provide immediate feedback.

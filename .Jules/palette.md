## 2025-05-21 - Inclusive Minute Filtering for Transit
**Learning:** Filtering scheduled departures using `>` instead of `>=` creates a 60-second "dead zone" where a train due within the current minute disappears from the UI before it actually departs, causing user confusion.
**Action:** Always use inclusive checks (`m >= currentMinute`) for transit countdowns to ensure "Due now" states are correctly displayed and the current departure remains visible.

## 2025-05-21 - Screen Reader Context Pattern
**Learning:** Visual-only indicators (like background color changes for "Live" vs "Scheduled" status) are inaccessible to screen reader users.
**Action:** Use a visually hidden element (`.sr-only`) that updates its text content alongside visual changes to provide semantic state information to assistive technologies, and mark decorative indicators with `aria-hidden="true"`.

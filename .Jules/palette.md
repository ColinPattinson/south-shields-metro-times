## 2025-05-15 - Screen Reader Context Pattern
**Learning:** In a single-page app where status is indicated by color (e.g., Green for Live, Blue for Scheduled), screen reader users miss this critical context unless a visually hidden label (`.sr-only`) is updated alongside the visual change.
**Action:** Use a hidden span within the `aria-live` region to explicitly state the data source or status when the UI state changes.

## 2025-05-15 - Inclusive Time Filtering
**Learning:** Using `m > currentMinute` in time calculations creates a "dead zone" where a train due within the current minute is hidden until the minute rolls over, even though it is technically the "next" train.
**Action:** Use inclusive checks (`m >= currentMinute`) and map the 0-minute difference to a "Due now" state for better UX.

## 2024-05-24 - Inclusive Scheduling Logic
**Learning:** Using exclusive filters (e.g., `m > currentMinute`) for departure times creates a 60-second "dead zone" where a train due right now disappears from the UI before it has actually departed.
**Action:** Always use inclusive checks (`m >= currentMinute`) for real-time or scheduled countdowns to ensure "Due now" states are correctly displayed.

## 2024-05-24 - Screen Reader Context Pattern
**Learning:** Visual-only status indicators (like background color changes for "Live" vs "Scheduled" data) are invisible to screen readers.
**Action:** Implement a visually hidden span (`.sr-only`) that updates its text (e.g., "Live prediction:") alongside the visual change, and use `aria-live="polite"` to ensure the update is announced.

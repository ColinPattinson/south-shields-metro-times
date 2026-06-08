## 2026-06-08 - Screen Reader Context Pattern for Color-Coded Status
**Learning:** Using background colors (e.g., green for live, blue for scheduled) to convey status is inaccessible to screen reader and color-blind users unless accompanied by text.
**Action:** Implement a visually hidden `.sr-only` span that updates its text (e.g., "Live prediction:" vs "Scheduled departure:") alongside visual changes to provide equitable context.

## 2026-06-08 - Inclusive Minute Filtering in Transit Schedules
**Learning:** Using `m > currentMinute` when filtering scheduled departures creates a 60-second "dead zone" where a train departing within the current minute is hidden from the user.
**Action:** Use `m >= currentMinute` and map the 0-minute difference to a "Due now" state for better clarity and accuracy.

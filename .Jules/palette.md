## 2026-06-04 - Screen Reader Context Pattern
**Learning:** Color-coded status (e.g., Live vs. Scheduled) is invisible to screen reader and color-blind users unless paired with text. Using `aria-live` on a container with a visually hidden `sr-only` label allows for accessible status updates without cluttering the visual UI.
**Action:** Always include a visually hidden status label when using color to communicate state changes, and use `aria-live="polite"` for dynamic updates.

## 2026-06-04 - Schedule Filtering Dead Zones
**Learning:** Using exclusive filtering (e.g., `m > currentMinute`) for upcoming events creates a 60-second 'dead zone' where events happening within the current minute are hidden, even if they are still relevant (e.g., "Due now").
**Action:** Use inclusive checks (e.g., `m >= currentMinute`) for time-based filtering and implement a "Due now" state for zero-minute countdowns.

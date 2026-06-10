## 2025-05-14 - Screen Reader Context for State Changes
**Learning:** When using color as a primary indicator of state (e.g., green for live vs. blue for scheduled), screen reader users miss this context. Combining `aria-live="polite"` with a visually hidden `.sr-only` label that updates its text (e.g., "Live prediction:" vs. "Scheduled departure:") ensures the state is communicated effectively to all users.
**Action:** Use the "Screen Reader Context Pattern" (visually hidden label + aria-live) whenever a component's state is primarily communicated through visual styling like background color.

## 2025-05-14 - Inclusive Minute Filtering for Transit
**Learning:** Transit schedules should use inclusive filtering (`m >= currentMinute`) for the current minute. A strict "greater than" check creates a 60-second "dead zone" where a train due within the current minute disappears from the "next" list before it has actually departed.
**Action:** Always use inclusive checks for time-based filtering to ensure "Due now" states are reachable and accurate.

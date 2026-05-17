## 2024-05-17 - Screen Reader Context for Color-Coded States
**Learning:** When using color to communicate state (e.g., green for 'Live' vs blue for 'Scheduled'), visual-only indicators are insufficient for accessibility. Using a visually hidden element (`.sr-only`) that updates alongside the visual change ensures screen reader users receive the same information.
**Action:** Always pair color-based state changes with a corresponding `.sr-only` text label or ARIA attribute.

## 2024-05-17 - Inclusive Time Filtering for "Due Now" States
**Learning:** Standard time-remaining logic often uses strict inequality (m > currentMinute), which causes a "gap" where an item disappears exactly when it is due. Using inclusive inequality (m >= currentMinute) allows the UI to display a "Due now" state, providing better clarity for users.
**Action:** Use inclusive filtering for countdowns and implement a specific "Due now" string for 0-minute wait times.

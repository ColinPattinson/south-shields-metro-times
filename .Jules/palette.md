## 2026-05-22 - Screen Reader Context Pattern
**Learning:** Visual-only state indicators (like background colors for 'Live' vs 'Scheduled') are inaccessible to screen readers and color-blind users unless accompanied by text or specific ARIA attributes.
**Action:** Use a visually hidden span (`.sr-only`) that updates its text content alongside visual changes to provide equitable state information to all users.

## 2026-05-22 - Intuitive Transit Countdown
**Learning:** Displaying "0 mins" for a departing transit vehicle can be ambiguous and lacks urgency.
**Action:** Use "Due now" for zero-minute countdowns to provide immediate, clear, and actionable feedback to the user.

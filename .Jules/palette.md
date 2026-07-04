## 2026-07-04 - Fixing the Minute "Dead Zone" and Enhancing Time-Based UX
**Learning:** For countdowns or departure boards, using an exclusive "greater than" check for current-minute events (e.g., `m > currentMinute`) creates a 60-second window where the next event disappears before it actually occurs. Additionally, displaying "Due now" instead of a timestamp or "0 mins" provides immediate, high-confidence feedback to the user.
**Action:** Always use inclusive checks (`>=`) for current-time comparisons and implement a specific "Due now" state for zero-minute durations.

## 2026-07-04 - High-Contrast Branding for Accessibility
**Learning:** Standard "UI blue" (#3498db) and "UI green" (#27ae60) often fail WCAG AA contrast ratios (4.5:1) when used as backgrounds for small white text or as status indicators on white backgrounds.
**Action:** Use verified accessible alternatives like #1b7a43 (Green) and #206694 (Blue) for status indicators and high-impact UI elements to ensure visibility for all users.

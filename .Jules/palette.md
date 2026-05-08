## 2025-05-14 - Screen Reader Context Pattern
**Learning:** For dynamic UI updates that use color to convey state (like live vs scheduled data), simply changing the background color is insufficient for accessibility. Using an `aria-live="polite"` container combined with a visually hidden `.sr-only` span that updates its text (e.g., "Live departure: ") ensures that screen reader users receive the same context as visual users.
**Action:** Always pair visual state changes (color, icons) with a visually hidden text label in an aria-live region.

## 2025-05-14 - Robust Relative Time Displays
**Learning:** Displaying "0 mins" for immediate events can be confusing. "Due now" provides much better user clarity for transit applications. Additionally, relative time calculations must account for midnight wrap-around (adding 1440 minutes if the difference is negative) to avoid incorrect negative offsets.
**Action:** Implement "Due now" logic for 0-minute states and always include modulo/day-wrap logic for time-of-day calculations.

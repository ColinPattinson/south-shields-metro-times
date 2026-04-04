## 2025-05-14 - Pluralization and Immediate States in Transit Countdowns
**Learning:** Transit countdowns are more intuitive when they display "Due now" for 0-minute waits and use correct pluralization (min vs mins) for other values.
**Action:** Always implement conditional logic for time-based displays: `minsUntil === 0 ? 'Due now' : `${minsUntil} ${minsUntil === 1 ? 'min' : 'mins'}``.

## 2025-05-14 - Screen Reader Visibility for Dynamic Content
**Learning:** Dynamic updates in single-page applications are often missed by screen readers unless explicitly marked with `aria-live="polite"`.
**Action:** Ensure all elements that update via JavaScript (timers, status indicators, analysis results) have appropriate ARIA live regions.

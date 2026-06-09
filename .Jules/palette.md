## 2026-06-09 - Enhanced Accessibility & Status Feedback
**Learning:** For time-sensitive information, using color-coded states (Live vs. Scheduled) requires accompanying text labels for accessibility (WCAG AA). "Due now" provides a clearer micro-UX than "0 mins".
**Action:** Always pair visual indicators with aria-live and sr-only labels to ensure equal information access for screen reader users. Use CSS classes instead of hardcoded style manipulation for better maintainability.

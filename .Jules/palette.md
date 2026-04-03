## 2025-05-14 - Transit Countdown Clarity and Accessibility
**Learning:** For countdowns or time-until displays, users appreciate "Due now" instead of "0 mins" for clarity. Additionally, ensuring screen readers receive updates via `aria-live` and have semantic context for status indicators via `role="img"` and `aria-label` significantly improves accessibility.
**Action:** Always implement conditional pluralization and "Due now" labels in countdowns. Use `aria-live="polite"` for dynamic content sections and provide descriptive `aria-label` for color-coded status elements.

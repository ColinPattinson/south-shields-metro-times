## 2025-05-15 - Screen Reader Context Pattern
**Learning:** Screen readers often miss state changes communicated solely through color (e.g., background-color changes). Using a visually hidden span (`.sr-only`) that updates its text alongside visual changes ensures assistive technology users receive the same context (e.g., "Live" vs "Scheduled").
**Action:** Always include an `.sr-only` context label when using color to indicate status or data source.

## 2025-05-15 - Precise Time Pluralization and Immediacy
**Learning:** "0 mins" is less intuitive than "Due now", and "1 mins" is grammatically incorrect. Micro-copy improvements like correct pluralization and status-specific phrases significantly enhance the "polish" of transit apps.
**Action:** Use conditional logic for time-based labels to handle singular/plural and immediate states.

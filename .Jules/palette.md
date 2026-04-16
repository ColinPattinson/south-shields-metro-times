## 2025-04-16 - Screen Reader Context for Dynamic States
**Learning:** For UIs that use color to communicate state (e.g., green for live data, blue for scheduled data), screen reader users miss this context. A visually hidden span (`.sr-only`) that updates its text based on the source provides the same context to assistive technology without affecting the visual layout.
**Action:** Always provide a text-based equivalent for state communicated through color or icons.

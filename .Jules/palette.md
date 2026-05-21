## 2026-05-21 - Screen Reader Context Pattern for Visual States
**Learning:** For single-page apps that use background colors or icons to communicate state (e.g., "Live" vs "Scheduled"), using a visually hidden span (`.sr-only`) with `aria-live="polite"` on the parent allows screen reader users to receive immediate, contextual updates without interrupting their flow.
**Action:** Always pair visual-only state indicators (background colors, status dots) with an `.sr-only` text label and ensure the parent container has appropriate `aria-live` attributes.

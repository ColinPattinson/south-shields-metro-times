## 2026-05-29 - Screen Reader Context for Dynamic Color States
**Learning:** When using color (e.g., Green for 'Live', Blue for 'Scheduled') to communicate application state, screen reader users miss this context. Combining `aria-live="polite"` with a visually hidden (`.sr-only`) label that explicitly states the status ensures all users receive the same information when the UI updates.
**Action:** Use the 'Screen Reader Context Pattern': a parent container with `aria-live` and a child `.sr-only` span that updates its text alongside visual changes.

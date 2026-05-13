## 2026-05-13 - Screen Reader Context Pattern
**Learning:** Purely visual cues like background color changes (e.g., green for Live, blue for Scheduled) are invisible to screen reader users. The 'Screen Reader Context Pattern' uses a visually hidden `.sr-only` element to provide this missing state information in text form.
**Action:** Always pair visual state changes with a hidden text alternative and use `aria-live` to ensure the update is announced when the state changes dynamically.

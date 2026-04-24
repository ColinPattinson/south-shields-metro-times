## 2025-05-14 - Screen Reader Context Pattern
**Learning:** For dynamic, color-coded status elements, visual users get immediate feedback via color, but screen reader users may miss the *source* or *state* of the data if only the value (time) is updated. Adding a visually hidden label that describes the state (e.g., "Live" vs "Scheduled") within an `aria-live` region ensures parity.
**Action:** Always include a `.sr-only` context label in dynamic status containers that use color to convey meaning.

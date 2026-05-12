# Palette's Journal - Critical UX/Accessibility Learnings

This journal is strictly for critical UX/accessibility learnings (patterns, surprises, or reusable insights).

## 2025-05-14 - Screen Reader Context Pattern
**Learning:** Using `aria-live="polite"` on a container that includes both a visually hidden label (`.sr-only`) and a dynamic value ensures that screen reader users receive context for updates (e.g., "Live departure: 09:41") rather than just hearing the time.
**Action:** Always wrap dynamic values in a container with a descriptive, visually hidden label when the value's meaning depends on visual cues like color.

# Palette's Journal - South Shields Metro Times

## 2026-05-16 - Screen Reader Context Pattern
**Learning:** Purely visual indicators (like background color changes or colored dots) are invisible to screen reader users. Simply adding `aria-live` to a container isn't enough if the *meaning* of the change isn't conveyed in text.
**Action:** Use a "Screen Reader Context Pattern": a visually hidden span (`.sr-only`) that updates its text (e.g., "Live" vs "Scheduled") alongside the visual change. This ensures all users understand the provenance of the data.

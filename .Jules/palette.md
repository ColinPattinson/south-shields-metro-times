## 2025-05-14 - Textual Context for Color-Coded Status
**Learning:** Using background colors (green/blue) to indicate data source (live/scheduled) is intuitive for sighted users but invisible to screen readers. Providing a visually hidden label within an aria-live region ensures all users are informed of the data's reliability.
**Action:** Always accompany color-based state changes with a hidden text label and consider using aria-live to announce these changes.

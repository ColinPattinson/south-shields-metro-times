# Palette's Journal - Critical Learnings Only

## 2025-05-15 - Screen Reader Context Pattern
**Learning:** Color-coded states (like green for live, blue for scheduled) and decorative indicators (like status dots) are invisible to screen reader users and can be ambiguous for color-blind users.
**Action:** Use a `.sr-only` class to provide visually hidden text that describes the state or indicator (e.g., "Live prediction:" or "Service status: info").

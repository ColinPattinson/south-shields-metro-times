## 2026-04-17 - Accessible Color Contrast & Screen Reader Context
**Learning:** Standard UI colors like #3498db and #27ae60 often fail WCAG contrast requirements when paired with white text. Additionally, visual state changes (like color shifts to indicate live vs static data) are invisible to screen readers without explicit text context.
**Action:** Always use darker, accessible color variants (e.g., #1565c0 for blue, #1b5e20 for green) and provide hidden context spans (.sr-only) to describe the state change to assistive technology users.

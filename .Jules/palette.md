## 2026-04-29 - Accessible Transit Countdowns
**Learning:** For time-sensitive transit applications, "Due now" provides better UX than "0 mins". Additionally, using aria-live="polite" on parent containers ensures that screen readers announce both the label and the dynamic update together, providing necessary context.
**Action:** Always implement a "Due now" state for 0-minute countdowns and prefer aria-live on context-rich parent elements rather than just the dynamic value span.

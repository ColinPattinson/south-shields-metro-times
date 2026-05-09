## 2026-05-09 - Decoupling manual refresh UI from background auto-refresh
**Learning:** In applications with both automatic and manual refresh mechanisms, sharing the same update function that modifies UI state (like disabling a button) can lead to unexpected interface locking or visual flickering during background tasks.
**Action:** Always parameterize the update function (e.g., `isManual`) to ensure visual loading indicators only appear in response to explicit user intent, preserving "invisible" background updates.

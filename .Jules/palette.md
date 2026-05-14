## 2024-05-14 - Accessible Status Communication
**Learning:** Background colors alone (e.g., green for 'Live', blue for 'Scheduled') are insufficient for accessibility as they don't communicate state to screen readers or users with color blindness.
**Action:** Use a visually hidden label (.sr-only) that updates its text content alongside visual state changes, and ensure the parent container uses aria-live="polite" to announce these changes automatically.

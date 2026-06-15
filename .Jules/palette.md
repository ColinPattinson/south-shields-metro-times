## 2025-05-15 - Fixing the 'Dead Zone' in Transit Timetables
**Learning:** In transit apps, using an exclusive 'greater than' check (m > currentMinute) for scheduled departures creates a 60-second 'dead zone' where the current departure disappears before it actually leaves.
**Action:** Always use an inclusive check (m >= currentMinute) and provide a specific 'Due now' state for 0-minute wait times to ensure continuity and clarity for the user.

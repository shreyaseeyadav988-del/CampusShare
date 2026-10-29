# CampusShare — Emergency MVP
A client-side prototype for sharing campus practice rooms, sports facilities, equipment and books.

## Run
Extract the ZIP and open `index.html` in a modern browser. No install/build step required.

## Judge test (full journey)
1. In Student view, open DSLR Camera Kit and request a slot. Purpose: `Photography for campus fest`; duration: `2 hours; return by 5 PM`.
2. Open Staff view and approve the request.
3. Switch to Student view > My bookings > Check in / collect. Enter `Good; no visible damage`.
4. Click Return resource. Enter `Returned in good condition`; choose No when asked to report an issue.
5. Open Activity history and verify request, approval, check-in and return events.
6. Test conflict handling by requesting the same resource and slot again.
7. Test incident handling by returning an item and choosing Yes when asked to report an issue; staff can review it.

## Limitations (disclose honestly)
This is an emergency, browser-only prototype. It stores data in localStorage; it is not a real multi-user service. Student verification and role switching are simulated, not secure authentication. Availability and resources are fictional. Condition records use text, not uploaded photos. No server/database/email notifications are integrated. Never enter real personal data.

## Build and disclosure
Frontend: HTML, CSS, vanilla JavaScript. Storage: browser localStorage. No external libraries or AI APIs in this code. List AI assistance and any generated/pre-existing code accurately in the event disclosure, and ensure it complies with the official build-window rules.

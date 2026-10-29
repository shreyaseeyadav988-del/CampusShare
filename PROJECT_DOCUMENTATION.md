# CampusShare — Project Documentation

## Use case
A campus platform to discover and request practice rooms, sports facilities, portable equipment and books for student activities.

## Users
- Student: discover resources, review rules, request a slot, track status, check in/out and report an issue.
- Authorised staff: review requests, approve/reject/waitlist, prevent scheduling conflicts and review reported issues.

## Problem rationale
Students may need campus spaces or equipment for rehearsals, events, projects and sports activities. Informal coordination can make availability, approval and return accountability difficult. This is the product rationale and should be validated with local student/staff interviews.

## Solution and workflow
1. Student selects a resource and reviews location, rules and available slots.
2. Student submits purpose, slot, duration and a fictional demo ID.
3. Prototype checks for an existing pending/approved/checked-out booking for the same resource and slot.
4. Request becomes pending or waitlisted.
5. Staff approves, rejects or waitlists. Conflicting approvals are blocked.
6. Student records initial condition at check-in.
7. Student records final condition at return and can report an issue.
8. Staff records a review outcome for reported issues.
9. Activity history records actions and timestamps.

## Features
Search and category filters; sample resource catalogue; purpose-based requests; simulated verification; student/staff views; approve/reject/waitlist; basic conflict prevention; condition text at handover and return; incident reporting; activity history; browser-local persistence; JSON export.

## Technology
Single-page frontend in `index.html`, using HTML, CSS and vanilla JavaScript. Persistence uses browser localStorage. There is no backend, external AI API or shared database in this emergency MVP.

## Security, fairness and privacy
Demo data only. Simulated verification and role switching are not secure authentication. The browser-side conflict check is not safe for concurrent real users. Issues are recorded for human review; no automatic penalty is imposed. Production requires server-side authorisation, secure sessions, database transactions, institutional verification, privacy controls, file-upload validation and concurrency tests.

## Known limitations
Browser-local state; no multi-user sync; no real identity verification; no photo uploads; no email notifications; simplified waiting list and scheduling; fictional inventory/availability; no real penalty/deposit handling.

## Future work
Node/Express API, relational database, server-side roles, institutional sign-in, secure condition-photo uploads, calendar/notification integration, configurable fair allocation, accessibility and automated testing.

## Testing
Follow `TESTING.md`.

## Tools and contribution disclosure
Complete truthfully before submission. List the tools, AI assistance, libraries, hosting and code/templates actually used, and confirm compliance with event rules.

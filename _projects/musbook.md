---
title: MusBook Scheduling Platform
category: Product
order: 2
summary: Launched a full-stack platform for music lesson scheduling, messaging, and analytics used by students and staff at Dubai College.
timeline: Sep 2023 – May 2025
role: Founder & Full-Stack Developer
location: Dubai College
skills:
  - Django
  - Celery
  - Tailwind CSS
  - PostgreSQL
  - WebSockets
lead: Helping music departments run on-time lessons with automated logistics and delightful interfaces for teachers, students, and parents.
---

## From studio chaos to a structured flow
MusBook started as a personal frustration—ensembles were losing rehearsal time because lessons and accompanist bookings were all tracked manually. I interviewed teachers, accompanists, and students, then mapped each workflow on a giant kanban wall. The result was a unified scheduling platform with real-time messaging and automation baked in.

I shipped the MVP in six weeks using Django, PostgreSQL, and Tailwind. Celery workers sync timetables with Google Calendar, send reminders, and track instrument-specific attendance. WebSocket channels power responsive dashboards so teachers know who is in transit and which rooms are free.

## What I built
- **Role-aware portals:** Distinct dashboards for students, parents, accompanists, and staff with tailored permissions and analytics.
- **Automated logistics:** Stripe-powered invoicing, attendance insights, and conflict detection that alerts staff before double-bookings occur.
- **Communication layer:** Secure in-app messaging with conversation threads, escalation paths, and audit trails for safeguarding compliance.

## Outcomes
During the pilot at Dubai College the platform coordinated roughly 150 bookings each month and lifted on-time lesson starts by about 20%. The analytics dashboard surfaced under-utilized rehearsal rooms, helping the department extend practice hours without adding staff.

## Continuing the journey
I'm currently preparing MusBook for a broader release by modularizing the scheduling engine, adding bulk-import tooling, and refining accessibility. The codebase now doubles as a teaching example for Logic Labs students who want to understand end-to-end product engineering.

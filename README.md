# Literacy Progress Tracker (Salesforce Declarative System)

![literary progress tracker logo](https://github.com/Rwb3n/lit_track/blob/main/logo1-sml.png)

## Overview

**Literacy Progress Tracker** is a fully declarative Salesforce-based application designed to monitor children's reading development and manage volunteer interactions without custom Apex code. The system emphasizes structured data capture, rapid session logging, progressive skill tracking, and minimal administrative overhead.

## Key Components

- **Student Management**: Centralized records for participants including demographics, program history, language, and status tracking.
- **Session Tracking**: Detailed logging of reading sessions, books read, volunteer support, and skill focus.
- **Assessment and Growth Metrics**: Structured recording of reading assessments, skill scores, confidence surveys, and milestone achievements.
- **Volunteer Coordination**: Assignment tracking, scheduling patterns, and volunteer contribution reporting.
- **Program Oversight**: Real-time dashboards and reports for administrators to monitor literacy outcomes and volunteer impact.

## Data Model Highlights

- Declaratively built around **master-detail** relationships for automatic roll-ups.
- Custom Metadata Type (**Book__c**) drives session standardization without excessive data entry.
- Roll-up fields and simple formulas replace complex Apex logic.
- Flows manage critical automations: intake, session logging, assessments, milestones.

## User Experience

- Guided **Flows** for student intake, session recording, and assessments to minimize user error.
- Optimized **Record Pages** with actionable layouts and key metrics surfaced immediately.
- Targeted **Dashboards** for student progress, program health, and volunteer management.

## Automation Strategy

- **Record-Triggered Flows** for automatic updates on reading levels, milestones, and student statuses.
- **Scheduled Flows** for weekly summaries, milestone reports, and volunteer reminders.
- **Screen Flows** for structured data capture without manual record creation.

## Implementation Approach

- Phased deployment over five weekends: Foundation → Sessions → Assessment → Volunteers → Milestones.
- Tight object-field relationships allow fast iteration and simple scalability.
- Built-in **scenario data generation** module for training, demos, and realistic testing.

## Security Model

- **Role-based access control** ensures sensitive student data is protected.
- Volunteers restricted to read/write access for only assigned sessions.

## Future Enhancements

- Parent-facing portals
- Mobile-optimized assessment entry
- Volunteer certification tracking
- Advanced book recommendation engines

## Design Principles

- **No Apex**: 100% Flow, formula, and configuration-driven.
- **Minimize Complexity**: Every formula and automation is designed to be maintainable by low-code admins.
- **Performance Awareness**: Object bloat, report filters, and record load optimizations are enforced.
- **Scalable Testability**: Scenario generator ensures system can be validated under near-realistic conditions.

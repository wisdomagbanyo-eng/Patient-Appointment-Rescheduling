# Patient Appointment Rescheduling System

## Context Diagram

```mermaid
flowchart LR
    Patient -->|Reschedule Request| AppointmentSystem
    AppointmentSystem -->|Updated Appointment Details| Patient

    AppointmentSystem -->|Appointment Rescheduled Event| NotificationService
    NotificationService -->|Notification| Patient

    AppointmentSystem -->|Appointment Information| HealthcareProvider
    HealthcareProvider -->|Updated Availability| AppointmentSystem

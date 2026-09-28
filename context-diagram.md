# Context Diagram

```mermaid
flowchart LR
    Patient -->|Reschedule appointment| AppointmentSystem
    AppointmentSystem -->|Updated appointment| Patient
    AppointmentSystem -->|Appointment change| NotificationService
    NotificationService -->|Notification| Patient
    AppointmentSystem -->|Appointment details| Doctor
    Doctor -->|Available time| AppointmentSystem

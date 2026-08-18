# Notify Service

Notify is the Government of BC’s enterprise notification service designed to send reliable, scalable, and consistent communications across multiple delivery channels such as Email, SMS, and third-party messaging systems.

With GC Notify being sunsetted, Notify provides a centralized platform for managing notifications across government systems.

---

## What Notify Does

Notify allows systems to:
- Send notifications via API
- Trigger event-driven communications
- Use reusable templates
- Track delivery status
- Integrate with external systems

---

## Key Features

- Multi-channel delivery (Email, SMS, Third-party)
- Template-based messaging
- Event-driven notifications
- Layered configuration system
- Callback and subscription support
- Notification tracking
- Preview before sending
- Attachment handling

---

## Core Design Principles

### 1. Multi-Tenancy
Each tenant operates independently with isolated:
- Templates
- Configurations
- Notification data

---

### 2. Layered Defaults

Configuration is applied in the following hierarchy:

1. Global Defaults  
2. Tenant Defaults  
3. Template Defaults  
4. Request Overrides  

This ensures flexibility while maintaining consistency.

---

### 3. Idempotency

Each notification request can include an idempotency key to prevent duplicate processing.

---

### 4. Asynchronous Processing

All notifications are processed asynchronously to ensure:
- Scalability
- Reliability
- Fault tolerance

---

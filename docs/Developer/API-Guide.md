# API Guide

## Endpoints

### POST /notifysimple
Send simple notifications

### POST /notifyevent
Trigger event-based notifications

### POST /preview
Preview notification

---

## Request Fields

- to
- templateId
- params
- overrides
- callbackUrl

---

## Response

```json
{
  "notifyId": "12345",
  "status": "QUEUED",
  "statusUrl": "/status/12345"
}
```

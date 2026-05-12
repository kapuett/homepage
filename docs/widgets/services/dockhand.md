---
title: Dockhand
description: Dockhand Widget Configuration
---

Learn more about [Dockhand](https://dockhand.pro/).

Note: The widget supports both Dockhand's **local** or bearer token auth.

**Allowed fields:** (max 4): `running`, `stopped`, `paused`, `total`, `cpu`, `memory`, `images`, `volumes`, `events_today`, `pending_updates`, `stacks`.
**Default fields:** `running`, `total`, `cpu`, `memory`.

```yaml
widget:
  type: dockhand
  url: http://localhost:3001
  environment: local # optional: name or id; aggregates all when omitted
  key: your-token # Use either token OR username/password
  username: your-user # required for local auth
  password: your-pass # required for local auth
```

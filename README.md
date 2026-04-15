# Retry Studio — Version Registry

Public version registry for Retry Studio resources. Used by scripts to check for updates at server boot.

## versions.json

```json
{
  "retry_inventory": "1.0.0",
  "retry_greenscreener": "1.0.0"
}
```

This file is updated automatically by GitHub Actions when a new release is published on any Retry Studio resource.

## How it works

1. A Retry resource publishes a new release (tag `v1.x.x`)
2. A GitHub Action in the private repo pushes the new version here
3. FiveM servers fetch `versions.json` at boot to check for updates

---

*Retry Studio — DayZ-style systems for FiveM*

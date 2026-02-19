# ClickUp Time Tracker — Chrome Extension

![Version](https://img.shields.io/badge/version-1.0.0-purple) ![Manifest](https://img.shields.io/badge/manifest-v3-blue) ![License](https://img.shields.io/badge/license-MIT-green)

A Chrome extension that lets you start and stop native ClickUp timers from any browser tab — no tab switching required. Built for teams that need fast, accurate time tracking across client projects without interrupting their workflow.

![Icon](assets/icon128.png)

---

## Features

- **Start timers from any tab** — entry name auto-fills from the active browser tab title
- **Searchable dropdowns** — type to filter from your full customer and project lists
- **Smart task switching** — shows project tasks when a project is selected, or general ad-hoc tasks otherwise
- **Billable flag** — mark entries billable at the point of capture
- **Mobile sync** — bidirectional sync with the ClickUp mobile app via native timer API
- **Recent timesheets panel** — last 10 entries with deep links into ClickUp
- **Auto-assignee** — automatically sets you as the owner of every time entry
- **Settings page** — view connected account, reset OAuth, refresh cache, toggle auto-assign

---

## Prerequisites

Before installing, your ClickUp workspace must be configured:

### ClickUp Workspace Structure
```
Customers (Space)
  └── Companies (List)       ← one Task per customer
  └── Ad Hoc Tasks (List)    ← Tech Support, Purchasing, Research, Administrative, Travel

Project Deliverables (Space)
  └── [Project Folder]       ← one Folder per project, with Tasks inside
  └── [Project Folder]
```

---

## Security Notes

- **Never commit `api/clickup.js` with real credentials** — add it to `.gitignore` or use environment substitution before distributing
- The Client Secret is embedded in the extension for internal use. If publishing publicly to the Chrome Web Store, move the token exchange to a backend server
- Each user's OAuth token is stored locally in their own `chrome.storage.local` — it never leaves their machine except in API calls to `api.clickup.com`

---

## Versioning

| Version | Notes |
|---|---|
| 1.0.0 | Initial release |

---

## Privacy

See [PRIVACY.md](PRIVACY.md) for full privacy policy.

---

## License

MIT — see [LICENSE](LICENSE) for details.

---

## Built By

[CERtaintech, LLC]

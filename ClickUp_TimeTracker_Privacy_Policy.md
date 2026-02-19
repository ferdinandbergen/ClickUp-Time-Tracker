# Privacy Policy — ClickUp Time Tracker Chrome Extension

**Last updated:** February 18, 2026
**Published by:** EnSight Technologies

---

## Overview

ClickUp Time Tracker is a Chrome extension that allows users to start and stop native ClickUp timers directly from any browser tab. This privacy policy explains what data the extension accesses, how it is used, and your rights regarding that data.

---

## Data We Collect

ClickUp Time Tracker collects only the minimum data necessary to function:

**ClickUp OAuth Access Token**
When you authorize the extension, ClickUp issues a personal access token. This token is stored locally in your browser using Chrome's built-in storage API (`chrome.storage.local`). It is used exclusively to authenticate API requests to ClickUp on your behalf.

**ClickUp User ID and Team ID**
Your ClickUp user ID and workspace (team) ID are retrieved at login and stored locally in Chrome storage. These are used to associate time entries with your account and to query your workspace data.

**Browser Tab Title**
When you open the extension, it reads the title of your currently active browser tab. This is used to auto-populate the "Entry Name" field as a convenience. This data is never stored or transmitted anywhere — it is only displayed in the extension popup for you to review and edit.

---

## How We Use Your Data

All data collected by this extension is used solely to provide time tracking functionality:

- Your OAuth token is used to make authenticated requests to the ClickUp API (api.clickup.com)
- Your user ID is used to assign time entries to your ClickUp account
- Your team ID is used to query your workspace's projects, tasks, and time entries
- Tab titles are used only to pre-fill the entry name field in the popup UI

**We do not:**
- Transmit your data to any server other than ClickUp's official API (api.clickup.com)
- Share your data with any third parties
- Use your data for advertising or analytics
- Store any data outside of your local Chrome browser storage
- Access your browsing history or any tab content beyond the active tab title

---

## Data Storage

All data stored by this extension lives locally on your device in Chrome's `chrome.storage.local`. This data is:

- Never synced to external servers by this extension
- Never accessible to any party other than you and the ClickUp API
- Automatically cleared when you reset your OAuth connection via Settings

---

## Third-Party Services

This extension communicates exclusively with **ClickUp's official API** at `https://api.clickup.com`. Your use of ClickUp is governed by ClickUp's own Privacy Policy and Terms of Service, available at [https://clickup.com/privacy](https://clickup.com/privacy).

---

## Data Retention and Deletion

You can remove all locally stored data at any time by:

1. Opening the extension
2. Clicking the **Settings** (⚙) icon
3. Clicking **Reset OAuth Connection**

This clears your OAuth token, user ID, team ID, and all cached data from Chrome storage. Uninstalling the extension also removes all locally stored data.

Time entries that have already been submitted to ClickUp are stored in your ClickUp workspace and are subject to ClickUp's own data retention policies.

---

## Permissions Explained

The extension requests the following Chrome permissions:

| Permission | Why It's Needed |
|---|---|
| `storage` | Store your OAuth token and cached data locally |
| `identity` | Handle the ClickUp OAuth authorization flow |
| `tabs` | Read the active tab title to pre-fill the entry name |
| `activeTab` | Access the currently active tab when the popup is open |
| `alarms` | Poll ClickUp every 30 seconds to sync timer state with mobile |
| `windows` | Open the ClickUp authorization window at a controlled size |

---

## Children's Privacy

This extension is intended for professional workplace use and is not directed at children under the age of 13. We do not knowingly collect data from children.

---

## Changes to This Policy

If this privacy policy is updated, the "Last updated" date at the top of this document will be revised. Continued use of the extension after changes constitutes acceptance of the updated policy.

---

## Contact

If you have questions about this privacy policy or the extension's data practices, please contact:

**EnSight Technologies**
info@certaintechllc.com

# Privacy Policy — QuickMark

**Last updated:** May 13, 2026

## Summary

QuickMark does not collect, transmit, or share any personal data. All information stays in your browser.

---

## Data Storage

QuickMark stores the following data locally in your browser using the Chrome Storage API:

- **Bookmarks** — URLs, names, and favicons of sites you add to Essentials or Favorites
- **Widget settings** — position, appearance preferences, opacity, blocked domains
- **Tab order** — your preferred section ordering in the popup

This data is stored in:
- `chrome.storage.sync` — synced across your Chrome-signed-in devices (subject to Chrome's 100KB quota)
- `chrome.storage.local` — local fallback when sync quota is exceeded

No data is stored on external servers.

---

## Network Requests

QuickMark makes exactly one type of external network request:

| Destination | Purpose | When |
|---|---|---|
| `https://www.google.com/s2/favicons` | Fetch site icons (favicons) for bookmarked URLs | When you add a new bookmark, and periodically to refresh stale icons |

- Favicons are fetched once, converted to data URLs, and cached locally
- No cookies or credentials are sent with these requests
- No user-identifiable information is transmitted
- No other external requests are made

---

## Data Collection

QuickMark does **NOT** collect:
- Personal information (name, email, address)
- Browsing history
- Page content
- Keystrokes or form data
- Analytics or usage telemetry
- Crash reports
- IP addresses
- Device identifiers

---

## Third-Party Services

QuickMark does **NOT** use:
- Analytics services (Google Analytics, Mixpanel, etc.)
- Advertising networks
- Error tracking services (Sentry, Bugsnag, etc.)
- Any third-party SDKs or libraries

The only external service contacted is Google's public Favicon Service, which serves pre-rendered site icons and does not track users.

---

## Data Sharing

QuickMark does **NOT** share data with:
- The extension developer
- Third parties
- Advertisers
- Data brokers
- Any external entity

---

## Data Export & Deletion

- **Export:** You can export all your data as a JSON file via Settings → Export Config
- **Delete:** Uninstalling the extension removes all stored data. You can also reset to defaults from Settings, which clears all custom bookmarks and preferences.

---

## Permissions Justification

| Permission | Justification |
|---|---|
| `storage` | Store bookmarks and settings locally and sync across devices |
| `contextMenus` | Add right-click menu options for quick bookmarking |
| `tabs` | Open bookmarked sites in new tabs; update context menu labels per page |
| `alarms` | Schedule periodic favicon refresh (every 24 hours) |
| `host_permissions: google.com/s2/favicons` | Fetch site icons from Google's favicon service |

---

## Children's Privacy

QuickMark does not knowingly collect information from children under 13. The extension does not collect information from anyone.

---

## Changes to This Policy

If this privacy policy changes, the updated version will be published in the extension's GitHub repository. The "Last updated" date at the top will reflect the most recent revision.

---

## Contact

For privacy-related questions, contact: [softrealms.com](https://softrealms.com)

# firebase-db-collection-schema
Reference repo for storing db schema

ToDo: Add existing and actively used collections into this repo.

## Collection Index

### interactions/

| Collection | Started | Last Activity | Notes |
|-----------|---------|--------------|-------|
| `InteractionLog` | Jul 2025 | **Apr 2026** | A volunteer's outreach session. Linked to `HelpRequest` via `helpRequestDocIds`. |
| `HelpRequest` | Oct 2025 | **Mar 2026** | A specific person in need identified during an interaction. Linked to `InteractionLog` via `interactionLogDocId`. |
| `helpRequests` | May 2024 | Jun 2025 — Deprecated | Public help request postings — volunteers or people in need describing someone requiring outreach. Superseded by `HelpRequest`. |
| `helpRequestsAndroid` | Apr 2024 | Jul 2024 — Deprecated | Android variant of `helpRequests`. |

### Outreaches/

| Collection | Started | Last Activity | Notes |
|-----------|---------|--------------|-------|
| `outreachEvents` | Oct 2023 | **Mar 2026** | Scheduled volunteering events (web/iOS). |
| `outreachEventsAndroid` | Oct 2023 | Sep 2024 — Deprecated | Android variant of `outreachEvents`. |
| `pastOutreachEvents` | Nov 2023 | Nov 2023 — Archived | Completed/past outreach events. |

### VisitLogs/

| Collection | Platform | Started | Last Activity | Notes |
|-----------|----------|---------|--------------|-------|
| `VisitLogBook_New` | iOS/Android | Nov 2022 | Feb 2026 — Deprecated | Predecessor to `InteractionLog` (mobile). Superseded but still seeing some writes. |
| `VisitLogBook` | iOS/Android | May 2023 | Aug 2025 — Deprecated | Earlier predecessor to `InteractionLog` (mobile). |
| `visitLogWebProd` | Web | Nov 2022 | Sep 2025 — Deprecated | Predecessor to `InteractionLog` (web). Superseded but still seeing some writes. |
| `personalVisitLog` | Web | Jan 2024 | Jul 2025 | Personal outreach log. |
| `visitLog` | Web | Apr 2023 | Jul 2023 — Deprecated | Earlier web visit log. |
| `pastVisitLogs` | Web | Sep 2023 | Sep 2023 — Archived | Archived web visit logs. |
| `visitLogs` | Web | Oct 2020 | May 2021 — Deprecated | Earliest structured visit logs; uses capitalized field names (`Date`, `Hours`, `Name`). |

### Metrics/
- **`Metrics`** — Aggregated metrics for homepage and community pages.

# OpsGenie (opsgenie)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

OpsGenie is an incident management and alerting platform, now part of Atlassian, that helps operations teams manage on-call schedules, route alerts, and coordinate incident response. The OpsGenie developer platform provides a comprehensive set of REST APIs for programmatically managing alerts, incidents, teams, schedules, escalations, integrations, heartbeats, services, notification rules, accounts, and maintenance windows.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- Alerts
- Incident Management
- Monitoring
- On-Call
- Operations

## Timestamps

- **Created:** 2025-03-01
- **Modified:** 2026-05-19

## APIs

### OpsGenie Alert API

Programmatically create, update, close, and manage alerts within the OpsGenie incident management platform. Alert creation, deletion, and action requests are processed asynchronously to provide higher availability and scalability. Supports alert priorities, responders, tags, custom details, notes, and acknowledgments.

- **Human URL:** [https://docs.opsgenie.com/docs/alert-api](https://docs.opsgenie.com/docs/alert-api)
- **Base URL:** `https://api.opsgenie.com`

#### Tags

- Alerts
- Incident Management
- Monitoring
- Notifications

#### Properties

- [Documentation](https://docs.opsgenie.com/docs/alert-api)
- [OpenAPI](openapi/opsgenie-alert-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opsgenie-alert.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opsgenie-alert.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/opsgenie-alert-schema.json) — [JSON Schema](https://json-schema.org/specification)

### OpsGenie Incident API

Create and manage incidents programmatically. Supports defining responders, tags, custom details, priority levels, and impacted services for each incident. Available to Standard and Enterprise plan users with endpoints for creating, updating, closing, and resolving incidents in a structured response workflow.

- **Human URL:** [https://docs.opsgenie.com/docs/incident-api](https://docs.opsgenie.com/docs/incident-api)
- **Base URL:** `https://api.opsgenie.com`

#### Tags

- Incidents
- Incident Management
- Operations
- Response

#### Properties

- [Documentation](https://docs.opsgenie.com/docs/incident-api)
- [OpenAPI](openapi/opsgenie-incident-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opsgenie-incident.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opsgenie-incident.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/opsgenie-incident-schema.json) — [JSON Schema](https://json-schema.org/specification)

### OpsGenie User API

Manage user accounts within the OpsGenie platform. Create, retrieve, update, and delete users, list users, and retrieve escalations associated with specific users. Supports managing user roles, contact methods, and notification preferences.

- **Human URL:** [https://docs.opsgenie.com/docs/user-api](https://docs.opsgenie.com/docs/user-api)
- **Base URL:** `https://api.opsgenie.com`

#### Tags

- Users
- Accounts
- Identity
- Management

#### Properties

- [Documentation](https://docs.opsgenie.com/docs/user-api)
- [OpenAPI](openapi/opsgenie-user-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opsgenie-user.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opsgenie-user.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### OpsGenie Team API

Manage teams within the OpsGenie platform. Create, update, retrieve, and delete teams, manage team members and their roles. Teams are a core organizational unit used to route alerts and assign on-call responsibilities to groups of users.

- **Human URL:** [https://docs.opsgenie.com/docs/team-api](https://docs.opsgenie.com/docs/team-api)
- **Base URL:** `https://api.opsgenie.com`

#### Tags

- Teams
- Groups
- Collaboration
- Management

#### Properties

- [Documentation](https://docs.opsgenie.com/docs/team-api)
- [OpenAPI](openapi/opsgenie-team-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opsgenie-team.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opsgenie-team.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### OpsGenie Schedule API

Programmatically manage on-call schedules and rotations. Create, update, and delete schedules, manage rotations and overrides, and query who is currently on call. Enables custom dashboards and integrations that reflect real-time on-call status.

- **Human URL:** [https://docs.opsgenie.com/docs/schedule-api](https://docs.opsgenie.com/docs/schedule-api)
- **Base URL:** `https://api.opsgenie.com`

#### Tags

- Schedules
- On-Call
- Rotations
- Planning

#### Properties

- [Documentation](https://docs.opsgenie.com/docs/schedule-api)
- [OpenAPI](openapi/opsgenie-schedule-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opsgenie-schedule.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opsgenie-schedule.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### OpsGenie Escalation API

Manage escalation policies that define how alerts are routed when initial responders do not acknowledge them. Create, update, retrieve, and delete escalation configurations with rules defining sequence of notifications and configurable delay intervals.

- **Human URL:** [https://docs.opsgenie.com/docs/escalation-api](https://docs.opsgenie.com/docs/escalation-api)
- **Base URL:** `https://api.opsgenie.com`

#### Tags

- Escalations
- Routing
- Alerts
- Workflows

#### Properties

- [Documentation](https://docs.opsgenie.com/docs/escalation-api)
- [OpenAPI](openapi/opsgenie-escalation-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opsgenie-escalation.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opsgenie-escalation.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### OpsGenie Integration API

Programmatically manage integrations that connect OpsGenie with third-party monitoring, ticketing, and communication tools. Create, enable, disable, and configure integrations and their associated actions. Note that Zendesk, Slack, and Incoming Call integrations must be configured through the OpsGenie web interface.

- **Human URL:** [https://docs.opsgenie.com/docs/integration-api](https://docs.opsgenie.com/docs/integration-api)
- **Base URL:** `https://api.opsgenie.com`

#### Tags

- Integrations
- Connections
- Third Party
- Automation

#### Properties

- [Documentation](https://docs.opsgenie.com/docs/integration-api)
- [OpenAPI](openapi/opsgenie-integration-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opsgenie-integration.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opsgenie-integration.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/opsgenie-webhook-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

### OpsGenie Heartbeat API

Set up and manage heartbeat monitors that track the health and availability of systems and services. Heartbeats expect periodic pings from monitored systems and generate an alert when a ping is not received within the configured interval.

- **Human URL:** [https://docs.opsgenie.com/docs/heartbeat-api](https://docs.opsgenie.com/docs/heartbeat-api)
- **Base URL:** `https://api.opsgenie.com`

#### Tags

- Heartbeat
- Health Checks
- Monitoring
- Uptime

#### Properties

- [Documentation](https://docs.opsgenie.com/docs/heartbeat-api)
- [OpenAPI](openapi/opsgenie-heartbeat-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opsgenie-heartbeat.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opsgenie-heartbeat.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/opsgenie-heartbeat-schema.json) — [JSON Schema](https://json-schema.org/specification)

### OpsGenie Service API

Manage services within the OpsGenie platform. Services represent business-critical applications and components that can be associated with incidents to track impact. Used in conjunction with the Incident API to identify which services are affected during an outage.

- **Human URL:** [https://docs.opsgenie.com/docs/service-api](https://docs.opsgenie.com/docs/service-api)
- **Base URL:** `https://api.opsgenie.com`

#### Tags

- Services
- Service Catalog
- Operations
- Management

#### Properties

- [Documentation](https://docs.opsgenie.com/docs/service-api)
- [OpenAPI](openapi/opsgenie-service-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opsgenie-service.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opsgenie-service.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### OpsGenie Notification Rule API

Manage notification rules that control how and when users receive alert notifications. Create, update, and delete notification rules, including conditions, time restrictions, and notification channels such as email, SMS, push notifications, and voice calls.

- **Human URL:** [https://docs.opsgenie.com/docs/notification-rule-api](https://docs.opsgenie.com/docs/notification-rule-api)
- **Base URL:** `https://api.opsgenie.com`

#### Tags

- Notifications
- Rules
- Alerts
- Configuration

#### Properties

- [Documentation](https://docs.opsgenie.com/docs/notification-rule-api)
- [OpenAPI](openapi/opsgenie-notification-rule-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opsgenie-notification-rule.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opsgenie-notification-rule.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### OpsGenie Account API

Retrieve account-level information and configuration settings. Access details about an OpsGenie account including plan information and account metadata. Foundational API for administrative operations and account management.

- **Human URL:** [https://docs.opsgenie.com/docs/account-api](https://docs.opsgenie.com/docs/account-api)
- **Base URL:** `https://api.opsgenie.com`

#### Tags

- Accounts
- Administration
- Settings
- Configuration

#### Properties

- [Documentation](https://docs.opsgenie.com/docs/account-api)
- [OpenAPI](openapi/opsgenie-account-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opsgenie-account.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opsgenie-account.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### OpsGenie Maintenance API

Manage maintenance windows that suppress alert notifications during planned maintenance periods. Create, update, list, and delete maintenance windows with configurable time ranges and rules for which integrations or policies are affected.

- **Human URL:** [https://docs.opsgenie.com/docs/maintenance-api](https://docs.opsgenie.com/docs/maintenance-api)
- **Base URL:** `https://api.opsgenie.com`

#### Tags

- Maintenance
- Windows
- Scheduling
- Operations

#### Properties

- [Documentation](https://docs.opsgenie.com/docs/maintenance-api)
- [OpenAPI](openapi/opsgenie-maintenance-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opsgenie-maintenance.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opsgenie-maintenance.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/opsgenie)
- [Portal](https://docs.opsgenie.com/)
- [Documentation](https://docs.opsgenie.com/docs)
- [Website](https://www.atlassian.com/software/opsgenie)
- [Privacy Policy](https://www.atlassian.com/legal/privacy-policy)
- [Terms of Service](https://www.atlassian.com/legal/software-license-agreement)
- [Support](https://support.atlassian.com/opsgenie/)
- [Blog](https://www.atlassian.com/blog)
- [Login](https://app.opsgenie.com/auth/login)
- [Features](undefined)
- [L L Ms Txt](https://docs.opsgenie.com/llms.txt)

## Maintainers

**FN:** API Evangelist
**Email:** info@apievangelist.com

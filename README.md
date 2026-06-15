# OpsGenie (opsgenie)

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

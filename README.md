# OpsGenie (opsgenie)
OpsGenie is an incident management and alerting platform, now part of Atlassian, that helps operations teams manage on-call schedules, route alerts, and coordinate incident response. Their developer platform provides a comprehensive set of REST APIs for programmatically managing alerts, incidents, teams, schedules, escalations, integrations, and other operational resources.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/apis.yml)

## Scope

- **Type:** Contract
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags:

 - Incident Management, Alerts, On-Call, Monitoring, Operations

## Timestamps

- **Created:** 2025-03-01
- **Modified:** 2026-03-20

## APIs

### OpsGenie Alert API
The OpsGenie Alert API allows developers to programmatically create, update, close, and manage alerts within the OpsGenie incident management platform. Alert creation, deletion, and action requests are processed asynchronously to provide higher availability and scalability. The API supports setting alert priorities, adding responders such as teams, users, escalations, and schedules, attaching tags and custom details, and managing alert notes and acknowledgments.

**Human URL:** [https://docs.opsgenie.com/docs/alert-api](https://docs.opsgenie.com/docs/alert-api)


#### Tags:

 - Alerts, Incident Management, Monitoring, Notifications

#### Properties

- [Documentation](https://docs.opsgenie.com/docs/alert-api)
- [OpenAPI](openapi/opsgenie-alert-openapi.yml)

### OpsGenie Incident API
The OpsGenie Incident API enables developers to create and manage incidents programmatically. It supports defining responders, tags, custom details, priority levels, and impacted services for each incident. The Incident API is available to Standard and Enterprise plan users and provides endpoints for creating, updating, closing, and resolving incidents as part of a structured incident response workflow.

**Human URL:** [https://docs.opsgenie.com/docs/incident-api](https://docs.opsgenie.com/docs/incident-api)


#### Tags:

 - Incidents, Incident Management, Operations, Response

#### Properties

- [Documentation](https://docs.opsgenie.com/docs/incident-api)
- [OpenAPI](openapi/opsgenie-incident-openapi.yml)

### OpsGenie User API
The OpsGenie User API provides endpoints for managing user accounts within the OpsGenie platform. Developers can create, retrieve, update, and delete users, as well as list users and retrieve escalations associated with specific users. The API supports managing user roles, contact methods, and notification preferences to ensure the right people are reached during incidents.

**Human URL:** [https://docs.opsgenie.com/docs/user-api](https://docs.opsgenie.com/docs/user-api)


#### Tags:

 - Users, Accounts, Identity, Management

#### Properties

- [Documentation](https://docs.opsgenie.com/docs/user-api)
- [OpenAPI](openapi/opsgenie-user-openapi.yml)

### OpsGenie Team API
The OpsGenie Team API allows developers to manage teams within the OpsGenie platform programmatically. It provides endpoints for creating, updating, retrieving, and deleting teams, as well as managing team members and their roles. Teams are a core organizational unit in OpsGenie used to route alerts and assign on-call responsibilities to groups of users.

**Human URL:** [https://docs.opsgenie.com/docs/team-api](https://docs.opsgenie.com/docs/team-api)


#### Tags:

 - Teams, Groups, Collaboration, Management

#### Properties

- [Documentation](https://docs.opsgenie.com/docs/team-api)
- [OpenAPI](openapi/opsgenie-team-openapi.yml)

### OpsGenie Schedule API
The OpsGenie Schedule API enables developers to programmatically manage on-call schedules and rotations. It provides endpoints for creating, updating, and deleting schedules, as well as managing schedule rotations and overrides. Developers can query who is currently on call for a given schedule, making it possible to build custom dashboards and integrations that reflect real-time on-call status.

**Human URL:** [https://docs.opsgenie.com/docs/schedule-api](https://docs.opsgenie.com/docs/schedule-api)


#### Tags:

 - Schedules, On-Call, Rotations, Planning

#### Properties

- [Documentation](https://docs.opsgenie.com/docs/schedule-api)
- [OpenAPI](openapi/opsgenie-schedule-openapi.yml)

### OpsGenie Escalation API
The OpsGenie Escalation API allows developers to manage escalation policies that define how alerts are routed when initial responders do not acknowledge them. It provides endpoints for creating, updating, retrieving, and deleting escalation configurations. Escalation rules define the sequence of notifications sent to teams, users, and schedules with configurable delay intervals to ensure incidents are addressed in a timely manner.

**Human URL:** [https://docs.opsgenie.com/docs/escalation-api](https://docs.opsgenie.com/docs/escalation-api)


#### Tags:

 - Escalations, Routing, Alerts, Workflows

#### Properties

- [Documentation](https://docs.opsgenie.com/docs/escalation-api)
- [OpenAPI](openapi/opsgenie-escalation-openapi.yml)

### OpsGenie Integration API
The OpsGenie Integration API enables developers to programmatically manage integrations that connect OpsGenie with third-party monitoring, ticketing, and communication tools. It provides endpoints for creating, enabling, disabling, and configuring integrations and their associated actions. Note that the Integration API does not support Zendesk, Slack, or Incoming Call integrations, which must be configured through the OpsGenie web interface.

**Human URL:** [https://docs.opsgenie.com/docs/integration-api](https://docs.opsgenie.com/docs/integration-api)


#### Tags:

 - Integrations, Connections, Third Party, Automation

#### Properties

- [Documentation](https://docs.opsgenie.com/docs/integration-api)
- [OpenAPI](openapi/opsgenie-integration-openapi.yml)

### OpsGenie Heartbeat API
The OpsGenie Heartbeat API allows developers to set up and manage heartbeat monitors that track the health and availability of systems and services. Heartbeats work by expecting periodic pings from monitored systems, and when a ping is not received within the configured interval, OpsGenie generates an alert. The API provides endpoints for creating, updating, deleting, and pinging heartbeats, enabling automated health monitoring for infrastructure and applications.

**Human URL:** [https://docs.opsgenie.com/docs/heartbeat-api](https://docs.opsgenie.com/docs/heartbeat-api)


#### Tags:

 - Heartbeat, Health Checks, Monitoring, Uptime

#### Properties

- [Documentation](https://docs.opsgenie.com/docs/heartbeat-api)
- [OpenAPI](openapi/opsgenie-heartbeat-openapi.yml)

### OpsGenie Service API
The OpsGenie Service API enables developers to manage services within the OpsGenie platform. Services represent business-critical applications and components that can be associated with incidents to track their impact. The API provides endpoints for creating, updating, retrieving, and deleting services. The Service API is available to Standard and Enterprise plan users and is used in conjunction with the Incident API to identify which services are affected during an outage.

**Human URL:** [https://docs.opsgenie.com/docs/service-api](https://docs.opsgenie.com/docs/service-api)


#### Tags:

 - Services, Service Catalog, Operations, Management

#### Properties

- [Documentation](https://docs.opsgenie.com/docs/service-api)
- [OpenAPI](openapi/opsgenie-service-openapi.yml)

### OpsGenie Notification Rule API
The OpsGenie Notification Rule API allows developers to manage notification rules that control how and when users receive alert notifications. It provides endpoints for creating, updating, and deleting notification rules, including defining conditions, time restrictions, and notification channels such as email, SMS, push notifications, and voice calls. This API enables fine-grained control over notification behavior for individual users.

**Human URL:** [https://docs.opsgenie.com/docs/notification-rule-api](https://docs.opsgenie.com/docs/notification-rule-api)


#### Tags:

 - Notifications, Rules, Alerts, Configuration

#### Properties

- [Documentation](https://docs.opsgenie.com/docs/notification-rule-api)
- [OpenAPI](openapi/opsgenie-notification-rule-openapi.yml)

### OpsGenie Account API
The OpsGenie Account API provides endpoints for retrieving account-level information and configuration settings. Developers can use this API to access details about their OpsGenie account, including plan information and account metadata. It serves as a foundational API for administrative operations and account management within the OpsGenie platform.

**Human URL:** [https://docs.opsgenie.com/docs/account-api](https://docs.opsgenie.com/docs/account-api)


#### Tags:

 - Accounts, Administration, Settings, Configuration

#### Properties

- [Documentation](https://docs.opsgenie.com/docs/account-api)
- [OpenAPI](openapi/opsgenie-account-openapi.yml)

### OpsGenie Maintenance API
The OpsGenie Maintenance API allows developers to manage maintenance windows that suppress alert notifications during planned maintenance periods. It provides endpoints for creating, updating, listing, and deleting maintenance windows with configurable time ranges and rules for which integrations or policies are affected. This helps operations teams avoid unnecessary alerting during scheduled downtime.

**Human URL:** [https://docs.opsgenie.com/docs/maintenance-api](https://docs.opsgenie.com/docs/maintenance-api)


#### Tags:

 - Maintenance, Windows, Scheduling, Operations

#### Properties

- [Documentation](https://docs.opsgenie.com/docs/maintenance-api)
- [OpenAPI](openapi/opsgenie-maintenance-openapi.yml)

## Common Properties

- [Portal](https://docs.opsgenie.com/)
- [Documentation](https://docs.opsgenie.com/docs)
- [Website](https://www.atlassian.com/software/opsgenie)
- [PrivacyPolicy](https://www.atlassian.com/legal/privacy-policy)
- [TermsOfService](https://www.atlassian.com/legal/software-license-agreement)
- [Support](https://support.atlassian.com/opsgenie/)
- [Blog](https://www.atlassian.com/blog)
- [Login](https://app.opsgenie.com/auth/login)

## Maintainers

**FN:** API Evangelist

**Email:** info@apievangelist.com

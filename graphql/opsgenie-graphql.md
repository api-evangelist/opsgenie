# OpsGenie (Atlassian) GraphQL Schema

## Overview

OpsGenie is an incident management and alerting platform, now part of Atlassian, that helps operations teams manage on-call schedules, route alerts, and coordinate incident response. While OpsGenie currently exposes its capabilities through a REST API, this conceptual GraphQL schema represents the full surface area of the platform's domain model: alerts, incidents, schedules, escalations, teams, users, integrations, heartbeats, services, maintenance windows, and notification policies.

The schema is derived from the OpsGenie REST API documentation at https://docs.opsgenie.com/docs/api-overview and covers the following API areas:

- Alert API
- Incident API
- Schedule API
- Escalation API
- Team API
- User API
- Integration API
- Heartbeat API
- Service API
- Notification Rule API
- Account API
- Maintenance API

## Schema Source

- **Provider:** OpsGenie (Atlassian)
- **Base URL:** https://api.opsgenie.com
- **Documentation:** https://docs.opsgenie.com/docs/api-overview
- **Schema Type:** Conceptual GraphQL (derived from REST API)
- **Schema File:** opsgenie-schema.graphql

## Core Domain Types

### Alerts

The alert domain is the central feature of OpsGenie. Alerts are created from integrations or the API and routed to the appropriate responders based on escalation and notification policies.

- `Alert` - Top-level alert object with id, message, alias, source, priority, status, and responders
- `AlertDetails` - Extended alert metadata including description, tags, custom details, and notes
- `AlertStatus` - Enum representing open, acked, or closed states
- `AlertPriority` - Enum for P1 through P5 priority levels
- `AlertSource` - Source integration or user that created the alert
- `AlertResponder` - A team or user assigned to respond to an alert
- `AlertTag` - String tag applied to an alert for filtering and routing
- `AlertNote` - A note added to an alert by a user or integration
- `AlertAck` - Acknowledgment record for an alert
- `AlertClose` - Close action record for an alert
- `AlertSnooze` - Snooze record with end time
- `AlertAction` - Generic action taken on an alert
- `AlertCountPayload` - Result type for alert count queries

### Incidents

Incidents represent coordinated response efforts, available on Standard and Enterprise plans.

- `Incident` - Top-level incident object
- `IncidentDetails` - Extended incident metadata
- `IncidentStatus` - Enum for open, resolved, or closed states
- `IncidentImpactedServices` - Services impacted by the incident
- `IncidentTag` - Tag applied to an incident
- `IncidentNote` - Timeline note attached to an incident

### Services

- `Service` - Business service registered in OpsGenie
- `ServiceDetails` - Extended service metadata including owner team
- `ServiceTeam` - Team associated with a service
- `AffectedTeam` - Team impacted by an incident

### On-Call and Schedules

- `OnCall` - Current on-call participant for a schedule
- `OnCallParticipant` - User or team currently on call
- `Schedule` - On-call schedule definition
- `ScheduleDetails` - Extended schedule metadata with rotations
- `ScheduleRotation` - A rotation within a schedule
- `RotationType` - Enum for daily, weekly, or hourly rotations
- `RotationParticipants` - Users or teams participating in a rotation
- `TimeRestriction` - Time range restriction for a rotation
- `WeekdayRestriction` - Day-of-week restriction for a rotation

### Escalations

- `EscalationPolicy` - Named escalation policy
- `EscalationRule` - A rule within an escalation policy
- `EscalationCondition` - Condition that triggers an escalation step
- `EscalationDelay` - Delay configuration between escalation steps

### Teams

- `Team` - OpsGenie team object
- `TeamDetails` - Extended team metadata
- `TeamMember` - A member of a team with their role
- `TeamContactMethod` - Contact method for a team member

### Users

- `User` - OpsGenie user account
- `UserDetails` - Extended user profile
- `UserRole` - Enum for admin, user, or read-only roles
- `UserNotification` - Notification preference for a user

### Notifications and Policies

- `NotificationPolicy` - Policy controlling when and how notifications are sent
- `MaintenanceWindow` - Scheduled window for suppressing alerts

### Heartbeats

- `Heartbeat` - Heartbeat monitor definition
- `HeartbeatDetails` - Extended heartbeat metadata with ping history

### Integrations and Webhooks

- `Integration` - OpsGenie integration with a third-party tool
- `IntegrationDetails` - Extended integration configuration
- `WebhookConfig` - Webhook endpoint and payload configuration

### Authentication

- `APIKey` - OpsGenie API key for authentication
- `Token` - Authentication token

## Query Capabilities

The GraphQL schema exposes the following top-level queries:

- `alert(id: ID!)` - Fetch a single alert by ID
- `alerts(...)` - List alerts with filtering and pagination
- `alertCount(...)` - Count alerts matching a filter
- `incident(id: ID!)` - Fetch a single incident by ID
- `incidents(...)` - List incidents
- `schedule(id: ID!)` - Fetch a schedule by ID
- `schedules(...)` - List all schedules
- `whoIsOnCall(scheduleId: ID!)` - Get current on-call participants
- `escalation(id: ID!)` - Fetch an escalation policy
- `escalations(...)` - List escalation policies
- `team(id: ID!)` - Fetch a team by ID
- `teams(...)` - List teams
- `user(id: ID!)` - Fetch a user by ID
- `users(...)` - List users
- `service(id: ID!)` - Fetch a service by ID
- `services(...)` - List services
- `heartbeat(name: String!)` - Fetch a heartbeat monitor
- `heartbeats(...)` - List heartbeat monitors
- `integration(id: ID!)` - Fetch an integration by ID
- `integrations(...)` - List integrations
- `maintenanceWindow(id: ID!)` - Fetch a maintenance window
- `maintenanceWindows(...)` - List maintenance windows
- `account` - Fetch the current account details

## Mutation Capabilities

- `createAlert(...)` - Create a new alert
- `closeAlert(...)` - Close an alert
- `acknowledgeAlert(...)` - Acknowledge an alert
- `snoozeAlert(...)` - Snooze an alert
- `addAlertNote(...)` - Add a note to an alert
- `createIncident(...)` - Create an incident
- `closeIncident(...)` - Close an incident
- `resolveIncident(...)` - Resolve an incident
- `createSchedule(...)` - Create a schedule
- `updateSchedule(...)` - Update a schedule
- `deleteSchedule(...)` - Delete a schedule
- `createTeam(...)` - Create a team
- `addTeamMember(...)` - Add a member to a team
- `removeTeamMember(...)` - Remove a member from a team
- `createUser(...)` - Create a user
- `updateUser(...)` - Update a user
- `deleteUser(...)` - Delete a user
- `createHeartbeat(...)` - Create a heartbeat monitor
- `pingHeartbeat(...)` - Send a ping to a heartbeat monitor
- `createMaintenanceWindow(...)` - Create a maintenance window

## Authentication

OpsGenie uses API key authentication. All requests require a `GenieKey` passed in the `Authorization` header:

```
Authorization: GenieKey <apiKey>
```

## Rate Limits

- Alerts API: 60 requests/min standard, up to 10,000 requests/min for high-volume integrations
- All other endpoints: 600 requests/min per API key

## Regional Endpoints

- US: https://api.opsgenie.com
- EU: https://api.eu.opsgenie.com

# Change Requests

## Objective

This document records change requests related to the project, allowing tracking of changes to requirements, architecture, processes, schedule or scope.

The goal is to ensure that every relevant change is analyzed, approved and documented before its implementation.

---

# Change Process

Standard flow:

```text
Request
      ↓
Impact Analysis
      ↓
Approval
      ↓
Planning
      ↓
Implementation
      ↓
Tests
      ↓
Release
```

---

# Possible Statuses

| Status        | Description                          |
| ------------- | ------------------------------------ |
| Open          | Request recorded                     |
| Under Review  | Impact assessment in progress        |
| Approved      | Change approved                      |
| Rejected      | Change refused                       |
| Implemented   | Change completed                     |
| Cancelled     | Request closed without execution     |

---

# Evaluation Criteria

Every request shall assess:

* Scope impact;
* Schedule impact;
* Architecture impact;
* Quality impact;
* Security impact;
* Testing impact;
* Cost impact.

---

# Request Log

## CR-001

### General Information

| Field          | Value         |
| -------------- | ------------- |
| ID             | CR-001        |
| Request Date   | 06/10/2026    |
| Requester      | Product Owner |
| Status         | Implemented   |
| Priority       | High          |

### Description

Add a password recovery feature via email.

### Justification

Users have no mechanism to recover access to the platform.

### Impact Analysis

| Area     | Impact |
| -------- | ------ |
| Backend  | Medium |
| Flutter  | Medium |
| Angular  | Medium |
| Database | Low    |
| Tests    | Medium |

### Affected Requirements

* REQ-F-003

### Affected Test Cases

* TC-008
* TC-009

### Decision

Approved.

### Owner

Stephanye Castellano

### Implementation Date

06/20/2026

### Notes

Feature delivered in Release 0.1.0.

---

## CR-002

### General Information

| Field          | Value          |
| -------------- | -------------- |
| ID             | CR-002         |
| Request Date   | 06/25/2026     |
| Requester      | Technical Team |
| Status         | Approved       |
| Priority       | Medium         |

### Description

Replace simple authentication with JWT authentication.

### Justification

Improve security and compatibility between applications.

### Impact Analysis

| Area     | Impact |
| -------- | ------ |
| Backend  | High   |
| Flutter  | Medium |
| Angular  | Medium |
| Database | Low    |
| Tests    | High   |

### Affected Requirements

* RNF-001
* RNF-002

### Affected Test Cases

* TC-010
* TC-011
* TC-012

### Decision

Approved.

### Owner

Development Team

### Planned Date

07/15/2026

### Notes

Architecture documentation needs to be updated.

---

## CR-003

### General Information

| Field          | Value      |
| -------------- | ---------- |
| ID             | CR-003     |
| Request Date   | 07/01/2026 |
| Requester      | End User   |
| Status         | Rejected   |
| Priority       | Low        |

### Description

Add a custom theme per user.

### Justification

Improve visual experience.

### Impact Analysis

| Area     | Impact |
| -------- | ------ |
| Backend  | Low    |
| Flutter  | Medium |
| Angular  | Medium |
| Database | Low    |
| Tests    | Medium |

### Reason for Rejection

Feature outside the current product scope.

### Notes

May be reassessed in future versions.

---

# Template for a New Request

## CR-XXX

### General Information

| Field          | Value |
| -------------- | ----- |
| ID             |       |
| Request Date   |       |
| Requester      |       |
| Status         |       |
| Priority       |       |

### Description

Describe the requested change.

### Justification

Reason for the request.

### Impact Analysis

| Area     | Impact |
| -------- | ------ |
| Backend  |        |
| Flutter  |        |
| Angular  |        |
| Database |        |
| Tests    |        |

### Affected Requirements

* REQ-XXX

### Affected Test Cases

* TC-XXX

### Change Traceability

| Artifact | Identifier |
|-----------|-----------|
| Change Request | CR-002 |
| Related Requirements | RNF-001, RNF-002 |
| Related Test Cases | TC-010, TC-011, TC-012 |
| Related Architectural Decision | ADR-006 |
| Related Release | 0.2.0 |

### Decision

Approved / Rejected

### Owner

Owner name.

### Planned Date

DD/MM/YYYY

### Notes

Additional information.

---

# Indicators

The following metrics may be tracked:

| Indicator                      | Goal                   |
| ------------------------------ | ---------------------- |
| Open requests                  | Demand control         |
| Approved requests              | Product evolution      |
| Rejected requests              | Scope control          |
| Average approval time          | Process efficiency     |
| Average implementation time    | Productivity           |

---

# Change History

| Date       | Version | Description                  |
| ---------- | ------- | ---------------------------- |
| 06/04/2026 | 1.0     | Initial creation of the document |

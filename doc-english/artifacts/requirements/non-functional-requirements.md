# Non-Functional Requirements

## Objective

This document describes the system's non-functional requirements, establishing criteria for quality, performance, security, usability, compatibility and maintenance.

Non-functional requirements define **how the system should operate**, complementing the functional requirements that define **what the system should do**.

Each requirement has a unique identifier to allow traceability during development and testing.

---

# Conventions

## Priority

| Level  | Description                              |
| ------ | ---------------------------------------- |
| High   | Essential for system operation           |
| Medium | Important for experience and maintenance |
| Low    | Desirable, but not critical              |

## Status

| Status            | Description                              |
| ----------------- | ---------------------------------------- |
| Planned           | Requirement approved for development     |
| In Implementation | In the process of being met              |
| Validated         | Met and tested                           |
| Cancelled         | Removed from scope                       |

---

# Non-Functional Requirements

## RNF-001 - Authentication Security

### Description

The system shall protect user access through secure authentication.

### Priority

High

### Status

Planned

### Criteria

* Passwords shall not be stored in plain text.
* Passwords shall be stored using secure hashing algorithms.
* Access to protected areas shall require valid authentication.
* Expired sessions shall require a new login.

---

## RNF-002 - Response Time

### Description

The system shall respond to common operations within an acceptable time for the user.

### Priority

High

### Status

Planned

### Criteria

* Query operations shall respond within 3 seconds under normal conditions.
* Authentication operations shall respond within 5 seconds.
* The system shall display loading indicators for long operations.

---

## RNF-003 - Availability

### Description

The system shall remain available for use whenever possible.

### Priority

High

### Status

Planned

### Criteria

* The system shall be designed to minimize downtime.
* Critical failures shall be logged for later analysis.
* The system shall have error recovery mechanisms when applicable.

---

## RNF-004 - Compatibility

### Description

The system shall work on the platforms supported by the project.

### Priority

High

### Status

Planned

### Criteria

#### Web Application

* Compatible with Google Chrome.
* Compatible with Microsoft Edge.
* Compatible with Mozilla Firefox.

#### Mobile Application

* Compatible with Android.
* Compatible with iOS.

#### Desktop Application

* Compatible with Windows.

---

## RNF-005 - Usability

### Description

The system shall offer an intuitive and consistent interface.

### Priority

Medium

### Status

Planned

### Criteria

* Main flows shall require the fewest possible actions.
* Error messages shall be clear and understandable.
* Visual elements shall remain consistent across screens.
* The user shall receive visual feedback for performed actions.

---

## RNF-006 - Maintainability

### Description

The system shall be developed in a way that eases future evolution and fixes.

### Priority

High

### Status

Planned

### Criteria

* The code shall follow standards defined by the team.
* Features shall have automated tests.
* The architecture shall favor separation of concerns.
* Documentation shall be kept up to date.

---

## RNF-007 - Testability

### Description

The system shall allow efficient validation through automated and manual tests.

### Priority

High

### Status

Planned

### Criteria

* Business rules shall be decoupled from the interface.
* Components shall allow isolated testing.
* Critical features shall have test coverage.
* Test cases shall be traceable to requirements.

---

## RNF-008 - Log Recording

### Description

The system shall record relevant events for auditing and diagnosis.

### Priority

Medium

### Status

Planned

### Criteria

* Errors shall be logged.
* Authentication failures shall be logged.
* Critical events shall have enough information for investigation.
* Sensitive information shall not be recorded in logs.

---

## RNF-009 - Scalability

### Description

The architecture shall allow gradual growth of the system.

### Priority

Medium

### Status

Planned

### Criteria

* New modules can be added without significant impact on existing modules.
* The architecture shall favor modularization.
* The system shall allow evolution to multiple simultaneous users.

---

## RNF-010 - Backup and Recovery

### Description

The system data shall have mechanisms to protect against loss.

### Priority

High

### Status

Planned

### Criteria

* The data shall have a defined backup strategy.
* The restoration process shall be documented.
* Storage failures shall be identifiable.

---

# Non-Functional Requirement Categories

| Category             | Identifiers     |
| -------------------- | --------------- |
| Security             | RNF-001         |
| Performance          | RNF-002         |
| Availability         | RNF-003         |
| Compatibility        | RNF-004         |
| Usability            | RNF-005         |
| Maintainability      | RNF-006         |
| Testability          | RNF-007         |
| Auditing and Logs    | RNF-008         |
| Scalability          | RNF-009         |
| Backup and Recovery  | RNF-010         |

---

# Traceability

Non-functional requirements shall be linked to:

* Test cases;
* Quality metrics;
* System architecture;
* Test strategy.

Example:

| Requirement | Test Case   | Evidence              |
| ----------- | ----------- | --------------------- |
| RNF-001     | TC-SEC-001  | Authentication test   |
| RNF-002     | TC-PERF-001 | Performance test      |
| RNF-007     | TC-QA-001   | Test coverage         |

---

# Change History

| Date       | Version | Description                  |
| ---------- | ------- | ---------------------------- |
| 06/04/2026 | 1.0     | Initial creation of the document |

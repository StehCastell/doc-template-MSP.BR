# Risk Management

## Objective

This document aims to identify, assess, monitor and mitigate risks that may impact the development, quality, schedule, cost or operation of the system.

Risk management shall be performed continuously throughout the entire project life cycle.

---

# Evaluation Criteria

## Impact

| Level    | Description                                       |
| -------- | ------------------------------------------------- |
| Low      | Small impact on the project                       |
| Medium   | Moderate impact on schedule, quality or scope     |
| High     | Significant impact on the project                 |
| Critical | May compromise the delivery or system operation   |

---

## Probability

| Level  | Description           |
| ------ | --------------------- |
| Low    | Unlikely              |
| Medium | May occur             |
| High   | High chance of occurring |

---

# Risk Classification

The risk priority shall consider the combination of impact and probability.

| Impact   | Probability | Priority |
| -------- | ----------- | -------- |
| Low      | Low         | Low      |
| Medium   | Low         | Low      |
| Medium   | Medium      | Medium   |
| High     | Medium      | High     |
| High     | High        | Critical |
| Critical | High        | Critical |

---

# Risk Log

## RSK-001

### Information

| Field     | Value        |
| --------- | ------------ |
| ID        | RSK-001      |
| Category  | Planning     |
| Status    | Open         |
| Priority  | High         |

### Description

Development delay due to the project being executed by a single person.

### Impact

High

### Probability

High

### Mitigation

* Prioritize MVP features.
* Keep the backlog organized.
* Avoid starting multiple features simultaneously.

### Contingency Plan

Reduce the release scope and replan deliveries.

---

## RSK-002

### Information

| Field     | Value      |
| --------- | ---------- |
| ID        | RSK-002    |
| Category  | Technology |
| Status    | Open       |
| Priority  | Medium     |

### Description

Requirement changes during development.

### Impact

Medium

### Probability

High

### Mitigation

* Formalize requirements before implementation.
* Use acceptance criteria.
* Record changes in requirements documents.

### Contingency Plan

Reassess the schedule and update documentation.

---

## RSK-003

### Information

| Field     | Value       |
| --------- | ----------- |
| ID        | RSK-003     |
| Category  | Integration |
| Status    | Open        |
| Priority  | High        |

### Description

Integration failures between frontend and backend applications.

### Impact

High

### Probability

Medium

### Mitigation

* Create clear API contracts.
* Use Swagger/OpenAPI.
* Run integration tests regularly.

### Contingency Plan

Immediate fix of the impacted integrations.

---

## RSK-004

### Information

| Field     | Value    |
| --------- | -------- |
| ID        | RSK-004  |
| Category  | Quality  |
| Status    | Open     |
| Priority  | High     |

### Description

Defects not identified before publishing.

### Impact

High

### Probability

Medium

### Mitigation

* Run unit tests.
* Run integration tests.
* Run exploratory tests.
* Use a release checklist.

### Contingency Plan

Publish an emergency fix (hotfix).

---

## RSK-005

### Information

| Field     | Value          |
| --------- | -------------- |
| ID        | RSK-005        |
| Category  | Infrastructure |
| Status    | Open           |
| Priority  | Medium         |

### Description

Loss of code or documentation.

### Impact

High

### Probability

Low

### Mitigation

* Use GitHub.
* Make frequent commits.
* Keep documentation versioned.

### Contingency Plan

Recovery through the repository history.

---

## RSK-006

### Information

| Field     | Value    |
| --------- | -------- |
| ID        | RSK-006  |
| Category  | Security |
| Status    | Open     |
| Priority  | Critical |

### Description

Exposure of sensitive user data.

### Impact

Critical

### Probability

Medium

### Mitigation

* Use HTTPS.
* Use JWT authentication.
* Validate inputs.
* Apply security best practices.

### Contingency Plan

Immediate blocking of the vulnerability and communication to affected users.

---

# Closed Risks

## RSK-000

### Description

Technology stack choice.

### Status

Closed.

### Resolution

Defined technologies:

* Backend: .NET
* Mobile/Desktop Frontend: Flutter
* Web Frontend: Angular

---

# Monitoring

Risks shall be reviewed:

* At each new release.
* When there is a significant scope change.
* When a risk materializes.
* During planning reviews.

---

# Template for New Risks

## RSK-XXX

### Information

| Field     | Value |
| --------- | ----- |
| ID        |       |
| Category  |       |
| Status    |       |
| Priority  |       |

### Description

Describe the risk.

### Impact

Low / Medium / High / Critical

### Probability

Low / Medium / High

### Mitigation

Actions to reduce the probability or impact.

### Contingency Plan

Actions to be taken if the risk occurs.

---

# Change History

| Date       | Version | Description                  |
| ---------- | ------- | ---------------------------- |
| 06/04/2026 | 1.0     | Initial creation of the document |

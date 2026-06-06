# Architectural Decisions

## Objective

This document records the main architectural decisions adopted during the system's development.

Recording the decisions allows:

- Understanding the reason for the choices made.
- Easing future maintenance.
- Supporting the onboarding of new collaborators.
- Avoiding re-discussion of decisions already made.
- Ensuring technical traceability.

---

# How to Record a Decision

Each architectural decision must contain:

| Field | Description |
|---------|---------|
| ID | Unique identifier |
| Date | Decision date |
| Status | Proposed, Approved or Superseded |
| Context | Problem or need |
| Decision | Chosen solution |
| Justification | Reasons for the choice |
| Consequences | Positive and negative impacts |

---

# ADR-001

## Information

| Field | Value |
|---------|---------|
| ID | ADR-001 |
| Date | 06/04/2026 |
| Status | Approved |

### Title

Use Flutter for Mobile and Desktop applications.

### Context

The project needs to provide applications for mobile and desktop devices.

One concern is to reduce maintenance cost and avoid multiple code bases.

### Decision

Use Flutter for Mobile and Desktop development.

### Justification

- Code sharing.
- Lower maintenance effort.
- Established ecosystem.
- Good performance.
- Suitable for small teams.

### Consequences

#### Positive

- Lower development cost.
- Component reuse.
- Unified testing strategy.

#### Negative

- Dependency on the Flutter ecosystem.
- Some specific integrations may require native code.

---

# ADR-002

## Information

| Field | Value |
|---------|---------|
| ID | ADR-002 |
| Date | 06/04/2026 |
| Status | Approved |

### Title

Use Angular for the Web application.

### Context

The Web application shall support future growth and administrative features.

### Decision

Use Angular as the frontend framework.

### Justification

- Robust structure.
- Modular organization.
- Strong corporate adoption.
- Excellent integration with TypeScript.

### Consequences

#### Positive

- Better project organization.
- Ease of maintenance.
- Scalability.

#### Negative

- Steeper learning curve.
- More initial configuration.

---

# ADR-003

## Information

| Field | Value |
|---------|---------|
| ID | ADR-003 |
| Date | 06/04/2026 |
| Status | Approved |

### Title

Use .NET as the Backend platform.

### Context

The system needs a robust API to serve multiple clients.

### Decision

Use ASP.NET Core Web API.

### Justification

- Excellent performance.
- Strong corporate support.
- Mature ecosystem.
- Great integration with automated testing.

### Consequences

#### Positive

- Scalability.
- Ease of maintenance.
- Large availability of libraries.

#### Negative

- Hosting may be more expensive depending on the environment.

---

# ADR-004

## Information

| Field | Value |
|---------|---------|
| ID | ADR-004 |
| Date | 06/04/2026 |
| Status | Approved |

### Title

Adopt Clean Architecture in the Backend.

### Context

The system shall grow over time and maintain good organization.

### Decision

Implement the Backend following Clean Architecture principles.

### Justification

- Separation of concerns.
- Ease of testing.
- Greater decoupling.

### Consequences

#### Positive

- More organized code.
- Better maintenance.
- Greater ease of evolution.

#### Negative

- More complex initial structure.

---

# ADR-005

## Information

| Field | Value |
|---------|---------|
| ID | ADR-005 |
| Date | 06/04/2026 |
| Status | Approved |

### Title

Use Feature First architecture in the Frontend.

### Context

Organizing the system by layers tends to generate very large structures as the project grows.

### Decision

Organize Angular and Flutter by features.

### Justification

Structure based on the business domain:

```text
features
├── auth
├── users
├── orders
└── dashboard
```

### Consequences

#### Positive

- Better organization.
- Ease of locating code.
- Scalability.

#### Negative

- May generate duplication without standardization.

---

# ADR-006

## Information

| Field | Value |
|---------|---------|
| ID | ADR-006 |
| Date | 06/04/2026 |
| Status | Approved |

### Title

Use JWT for authentication.

### Context

The API will be consumed by multiple clients.

### Decision

Implement JWT-based authentication.

### Justification

- Widely adopted standard.
- Compatible with Web, Mobile and Desktop.
- Easy integration.

### Consequences

#### Positive

- Stateless architecture.
- Scalability.

#### Negative

- Need to control token expiration and renewal.

---

# ADR-007

## Information

| Field | Value |
|---------|---------|
| ID | ADR-007 |
| Date | 06/04/2026 |
| Status | Approved |

### Title

Use a Monorepository.

### Context

The project will initially be developed by a single person.

### Decision

Keep Backend, Frontend and Documentation in the same repository.

### Justification

```text
Project
├── Backend
├── Frontend
├── Documentation
└── Infrastructure
```

### Consequences

#### Positive

- Simplified management.
- Centralized versioning.
- Lower operational effort.

#### Negative

- The repository tends to grow over time.

---

# ADR-008

## Information

| Field | Value |
|---------|---------|
| ID | ADR-008 |
| Date | 06/04/2026 |
| Status | Approved |

### Title

Do not use Docker initially.

### Context

The project will be developed and maintained by a single person.

### Decision

Run applications directly in the development environment during the initial phases.

### Justification

- Reduced operational complexity.
- Lower learning curve.
- Agility to start the project.

### Consequences

#### Positive

- Less configuration effort.
- Simpler environment.

#### Negative

- Less standardization across environments.
- Docker may be needed in the future.

---

# Change History

| Date | Version | Description |
|---------|---------|---------|
| 06/04/2026 | 1.0 | Initial creation of the document |

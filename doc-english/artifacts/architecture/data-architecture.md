# Data Architecture

## Objective

Describe how data is organized, stored, processed and protected within the solution.

---

# Overview

This document presents the data architecture adopted by the project, including the main entities, information flows and responsibilities related to data management.

---

# Data Sources

| Identification | Type           | Purpose                  |
| -------------- | -------------- | ------------------------ |
| Main Database  | Relational     | Operational persistence  |
| External APIs  | Service        | Integrations             |
| Files          | CSV, JSON, XML | Import and export        |

---

# Data Flow

```text
Data Source
        ↓
Validation
        ↓
Processing
        ↓
Persistence
        ↓
Query and Exposure
```

---

# Main Entities

| Entity  | Description                       |
| ------- | --------------------------------- |
| User    | Represents the system users       |
| Product | Represents the registered items   |
| Order   | Represents performed transactions |

---

# Storage Rules

* Sensitive data must be protected.
* Backups must be performed periodically.
* Historical data must have a retention strategy.

---

# Data Security

* Role-based access control.
* Use of encryption when applicable.
* Audit logging for critical operations.

---

# Change History

| Date       | Version | Description            |
| ---------- | ------- | ---------------------- |
| DD/MM/YYYY | 1.0     | Document creation      |

# Test Cases

## Objective

This document aims to define the test cases used to verify and validate the system requirements.

The test cases ensure that the implemented features meet the defined functional and non-functional requirements, and provide traceability between requirements, implementation and validation.

---

# Conventions

## Identification

Test cases shall follow the pattern:

```text
TC-XXX
```

Examples:

```text
TC-001
TC-002
TC-003
```

Specific cases may use category prefixes:

```text
TC-FUNC-001  → Functional
TC-INT-001   → Integration
TC-E2E-001   → End-to-End
TC-SEC-001   → Security
TC-PERF-001  → Performance
```

---

# Test Case Template

| Field            | Description                                       |
| ---------------- | ------------------------------------------------- |
| ID               | Unique identifier                                 |
| Requirement      | Associated requirement                            |
| Title            | Short test name                                   |
| Type             | Functional, Integration, E2E, Security, Performance |
| Priority         | High, Medium or Low                               |
| Preconditions    | Required conditions                               |
| Steps            | Execution sequence                                |
| Expected Result  | Correct result                                    |
| Status           | Not Executed, Passed, Failed                      |

---

# Functional Test Cases

## TC-FUNC-001 - User Registration with Valid Data

### Requirement

REQ-001 - User Registration

### Type

Functional

### Priority

High

### Preconditions

* User not previously registered.

### Steps

1. Access the registration screen.
2. Enter a valid name.
3. Enter a valid email.
4. Enter a valid password.
5. Confirm registration.

### Expected Result

* Account successfully created.
* User receives a confirmation message.

### Status

Not Executed

---

## TC-FUNC-002 - Registration with an Existing Email

### Requirement

REQ-001 - User Registration

### Type

Functional

### Priority

High

### Preconditions

* Email already registered in the system.

### Steps

1. Access the registration screen.
2. Enter an already existing email.
3. Confirm registration.

### Expected Result

* Registration rejected.
* Message informing the email is already in use.

### Status

Not Executed

---

## TC-FUNC-003 - Login with Valid Credentials

### Requirement

REQ-002 - User Authentication

### Type

Functional

### Priority

High

### Preconditions

* Previously registered user.

### Steps

1. Access the login screen.
2. Enter a valid email.
3. Enter a valid password.
4. Confirm authentication.

### Expected Result

* Login performed successfully.
* User directed to the main area.

### Status

Not Executed

---

## TC-FUNC-004 - Login with Invalid Password

### Requirement

REQ-002 - User Authentication

### Type

Functional

### Priority

High

### Preconditions

* Registered user.

### Steps

1. Access the login screen.
2. Enter a valid email.
3. Enter an incorrect password.
4. Confirm authentication.

### Expected Result

* Login rejected.
* Error message displayed to the user.

### Status

Not Executed

---

# Integration Test Cases

## TC-INT-001 - Integration between Frontend and Login API

### Requirement

REQ-002 - User Authentication

### Type

Integration

### Priority

High

### Preconditions

* API available.
* Registered user.

### Steps

1. Perform login through the interface.
2. Send a request to the API.
3. Receive the authentication response.

### Expected Result

* API returns a valid authentication.
* Interface receives and processes the response correctly.

### Status

Not Executed

---

# E2E Test Cases

## TC-E2E-001 - Complete Registration and Login Flow

### Requirement

REQ-001
REQ-002

### Type

E2E

### Priority

High

### Preconditions

* User not registered.

### Steps

1. Perform registration.
2. Confirm registration.
3. Log in.
4. Access the main area.

### Expected Result

* Flow executed without errors.
* User authenticated at the end of the process.

### Status

Not Executed

---

# Non-Functional Test Cases

## TC-SEC-001 - Secure Password Storage

### Requirement

RNF-001 - Authentication Security

### Type

Security

### Priority

High

### Preconditions

* Registered user.

### Steps

1. Create a user.
2. Query the stored record.
3. Verify how the password is stored.

### Expected Result

* Password not stored in plain text.
* Password protected by a hashing algorithm.

### Status

Not Executed

---

## TC-PERF-001 - Authentication Response Time

### Requirement

RNF-002 - Response Time

### Type

Performance

### Priority

Medium

### Preconditions

* Operational environment available.

### Steps

1. Perform authentication.
2. Measure the response time.

### Expected Result

* Response time below the limit defined by the requirement.

### Status

Not Executed

---

# Execution Control

## Possible Statuses

| Status        | Description                       |
| ------------- | --------------------------------- |
| Not Executed  | Test not yet performed            |
| In Progress   | Test in progress                  |
| Passed        | Result as expected                |
| Failed        | Result different from expected    |
| Blocked       | Impediment to execution           |

---

# Traceability

All test cases shall be linked to the system requirements.

Example:

| Test Case   | Requirement      |
| ----------- | ---------------- |
| TC-FUNC-001 | REQ-001          |
| TC-FUNC-002 | REQ-001          |
| TC-FUNC-003 | REQ-002          |
| TC-FUNC-004 | REQ-002          |
| TC-INT-001  | REQ-002          |
| TC-E2E-001  | REQ-001, REQ-002 |
| TC-SEC-001  | RNF-001          |
| TC-PERF-001 | RNF-002          |

---

# Change History

| Date       | Version | Description                  |
| ---------- | ------- | ---------------------------- |
| 06/04/2026 | 1.0     | Initial creation of the document |

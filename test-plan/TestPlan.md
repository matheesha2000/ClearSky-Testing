# Test Plan for Real-Time Air Quality Monitoring Dashboard

## Overview
This test plan outlines the testing strategy for the **Real-Time Air Quality Monitoring Dashboard for Colombo**, a web-based application designed to visualize air quality data. The goal is to ensure the system meets functional requirements, performs reliably, and delivers a seamless user experience.

---

## Scope

### In Scope
#### Functional Testing
- User authentication for Monitoring Admins
- Sensor management
- Real-time and historical AQI data visualization
- Automated data generation
- Alert threshold configuration
- Public dashboard accessibility

#### Non-Functional Testing
- Performance testing
- Security testing
- Cross-browser compatibility
- Database integrity checks

### Out of Scope
- Hardware failure simulations
- Penetration testing
- Mobile app testing

---

## Quality Objectives
- Validate all functional requirements specified in the coursework.
- Identify and resolve critical bugs before submission.
- Ensure data accuracy and real-time updates.
- Confirm seamless integration between frontend, backend, and database.

---

## Roles and Responsibilities
| Role               | Responsibilities                                                                 |
|--------------------|---------------------------------------------------------------------------------|
| **Test Lead**      | Oversees test execution, reviews reports, coordinates with developers.          |
| **QA Testers**     | Execute test cases, log defects, verify fixes.                                  |
| **Developers**     | Fix reported bugs, optimize performance.                                        |
| **Database Admin** | Ensure data consistency and proper storage.                                     |

---

## Test Methodology
### Approach
A **Waterfall testing approach** will be used, following a sequential SDLC where testing begins after development is finalized.

### Test Levels
| Level                  | Description                                                                 |
|------------------------|-----------------------------------------------------------------------------|
| **Unit Testing**       | Validate individual functions.                                              |
| **Integration Testing**| Test API endpoints, database interactions, and map integrations.            |
| **System Testing**     | End-to-end validation of all features.                                      |
| **UAT**               | Final review by the team to confirm coursework requirements are met.        |

### Suspension & Resumption Criteria
- **Suspend testing if:**
    - A major defect blocks >50% of test cases.
    - Test environment fails.
- **Resume testing after:**
    - Critical fixes are deployed.
    - Environment is restored.

### Test Completeness
Testing is complete when:
- 100% of test cases are executed.
- All critical/priority bugs are resolved.
- UAT confirms readiness for submission.

---

## Test Deliverables
- Test Plan
- Test Cases

---

## Resource & Environment Needs
### Testing Tools
| Tool               | Purpose                                   |
|--------------------|-------------------------------------------|
| **Browser Dev Tools** | Debug frontend.                         |
| **phpMyAdmin**     | Manual database validation.               |
| **Excel**          | Test case tracking & defect logging.      |

### Test Environment
- **OS**: Windows 10/11, macOS
- **Browsers**: Chrome
- **Backend**: XAMPP (PHP)
- **Database**: MySQL

---

## Terms/Acronyms
| Term  | Definition                               |
|-------|------------------------------------------|
| **AQI** | Air Quality Index                       |
| **UAT** | User Acceptance Testing                 |
| **API** | Application Programming Interface       |

--- 

**Note**: This document serves as a guide for testing the dashboard. Updates may be made based on feedback or changes in requirements.
# Day 14 - Flow Governance

## Approval Workflow Examples

### 1. Course Creation Approval

Workflow:

* Faculty submits a new course proposal.
* Department Head reviews the course structure.
* Academic Committee verifies syllabus quality.
* Principal gives final approval.

After Approval:

* Course becomes available for student enrollment.

After Rejection:

* Proposal returns to faculty for correction.

---

### 2. Faculty Leave Request Approval

Workflow:

* Faculty submits leave request.
* HOD reviews leave balance and schedule impact.
* Principal approves long-duration leave.

After Approval:

* Leave is marked approved in the system.

After Rejection:

* Faculty receives rejection notification.

---

### 3. Student Scholarship Request Approval

Workflow:

* Student submits scholarship application.
* Scholarship Committee verifies eligibility.
* Finance Department confirms budget availability.
* Principal approves final request.

After Approval:

* Scholarship amount is processed.

After Rejection:

* Student receives rejection reason.

---

### 4. Budget Approval Workflow

Workflow:

* Department submits budget request.
* Finance Team reviews financial feasibility.
* Management approves high-value requests.

After Approval:

* Budget allocation is released.

After Rejection:

* Request is sent back for modification.

---

# Branching Flow Logic

## Attendance Monitoring Flow

### Decision Logic

* If attendance is less than 75%

  * Send warning email to student.

* If attendance is less than 60%

  * Send notification to parents.

* If attendance is less than 50%

  * Escalate issue to college administration.

### Decision Points

* Attendance percentage acts as the decision variable.
* Different branches are triggered based on attendance conditions.

### Triggered Actions

* Automated emails
* Parent notifications
* Administrative escalation
* Student counseling recommendations

---

# Governance Explanation

Enterprise systems cannot allow every employee to directly modify sensitive records because it creates serious business risks.

## Reasons for Governance

### Security

Important data must be protected from unauthorized access.

### Misuse Prevention

Employees may accidentally or intentionally change critical information.

### Approval Control

Large organizations require validation before applying important changes.

### Business Risk Reduction

Uncontrolled updates may cause:

* Financial loss
* Compliance violations
* Incorrect reporting
* Operational failures

### Auditability

Organizations must track:

* Who changed data
* When changes occurred
* Why approvals were given

Governance ensures accountability, transparency, and business stability.

---

# Reflection

Controlled workflows are important because enterprises manage sensitive business operations involving finance, employees, customers, and compliance requirements.

Without governance:

* Wrong approvals may happen
* Fraud risks increase
* Data inconsistency occurs
* Business operations become unreliable

Approval workflows and branching automation help organizations:

* enforce business rules,
* maintain security,
* improve accountability,
* and ensure smooth enterprise operations.

This module helped me understand how Salesforce automation supports enterprise-level governance and structured business processes.

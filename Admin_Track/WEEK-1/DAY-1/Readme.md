# Salesforce Administrator - Day 1: User Management

## Introduction to Salesforce Administrator

A Salesforce Administrator is responsible for managing and optimizing the Salesforce CRM platform to improve business efficiency, automate processes, maintain data security, and strengthen customer relationships.

Salesforce Administrators act as the bridge between business users and technology. They configure Salesforce without extensive coding, manage users and permissions, create reports and dashboards, maintain data quality, and ensure that employees have the right level of access to perform their jobs.

### Key Responsibilities

* User Management
* Security and Access Control
* Data Management
* Automation using Flows
* Reports and Dashboards
* Customization of Objects and Fields
* System Maintenance and Monitoring
* Supporting Business Processes

---

# Difference Between User, Role, Profile, and Permission Set

| Feature        | User                            | Role                       | Profile                       | Permission Set                    |
| -------------- | ------------------------------- | -------------------------- | ----------------------------- | --------------------------------- |
| Purpose        | Represents a person who logs in | Controls record visibility | Controls baseline permissions | Grants additional permissions     |
| Assigned To    | Individual user                 | Individual user            | Individual user               | Individual user                   |
| Number Allowed | Many users                      | One role per user          | One profile per user          | Multiple permission sets per user |
| Controls       | Login identity                  | Data access hierarchy      | Object, field, and app access | Extra permissions beyond profile  |
| Example        | Student, Faculty                | HOD, Principal             | Standard User                 | Attendance Manager Access         |

## User

A user is an individual who can log in to Salesforce. Every user has a username, profile, and optional role.

## Role

A role determines what records a user can view through the role hierarchy. Higher roles can typically view records owned by users below them.

## Profile

A profile defines a user's baseline permissions, including object access, field access, login hours, and application access.

## Permission Set

A permission set provides additional permissions without modifying a user's profile. Multiple permission sets can be assigned to the same user.

---

# College Security Design

Assume Vishnu Institute is implementing Salesforce.

## Access Matrix

| Role                     | Student Records    | Course Records     | Placement Records    | Attendance Records |
| ------------------------ | ------------------ | ------------------ | -------------------- | ------------------ |
| Student                  | View               | View               | View                 | View               |
| Faculty                  | View, Create, Edit | View               | View                 | Create, Edit       |
| Placement Officer        | View               | View               | Create, Edit, Delete | View               |
| HOD                      | View, Create, Edit | View, Create, Edit | View, Edit           | View, Edit         |
| Principal                | View All           | View All           | View All             | View All           |
| Salesforce Administrator | Full Access        | Full Access        | Full Access          | Full Access        |

---

# Administrator Access Risks

Suppose a student accidentally receives Salesforce Administrator access.

## Problems That Might Occur

### 1. Unauthorized Data Access

The student could access confidential information including:

* Student records
* Faculty records
* Placement information
* Internal institutional data

### 2. Data Modification

The student could:

* Edit attendance records
* Modify grades
* Change placement records
* Delete important data

### 3. Security Risks

The student could:

* Create new administrator accounts
* Reset passwords
* Change security settings
* Disable security controls

### 4. Compliance Issues

Unauthorized access may violate institutional policies and data privacy regulations.

## Prevention Methods

* Follow the Principle of Least Privilege.
* Assign only required permissions.
* Use Permission Sets instead of giving Administrator access.
* Regularly audit user permissions.
* Enable Multi-Factor Authentication (MFA).
* Monitor login history and user activity.
* Review role hierarchy periodically.

---

# Reflection

## Why Do Enterprise Systems Need Strong Access Control?

Enterprise systems store sensitive business and personal information. Strong access control ensures that users can only access the information necessary for their job responsibilities.

Benefits of strong access control include:

* Protects sensitive data from unauthorized access.
* Reduces security breaches and insider threats.
* Maintains data integrity and accuracy.
* Supports regulatory compliance requirements.
* Prevents accidental data modification or deletion.
* Improves accountability through audit trails.
* Ensures business continuity and operational security.

In Salesforce, access control is implemented through Profiles, Roles, Permission Sets, Sharing Rules, and Organization-Wide Defaults. Together, these mechanisms ensure that the right users have the right access at the right time.

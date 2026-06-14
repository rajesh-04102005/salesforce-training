# Day 4 - Security & Sharing Model

## What is OWD?

OWD (Organization-Wide Defaults) defines the baseline level of access that users have to records they do not own. It is the first level of record security in Salesforce.

Types:
- Private
- Public Read Only
- Public Read/Write
- Controlled by Parent

OWD is used to restrict record access and then open it up using roles and sharing rules.

---

## What is Role Hierarchy?

Role Hierarchy is a mechanism that allows users higher in the hierarchy to access records owned by users below them.

Benefits:
- Simplifies record sharing.
- Managers can access subordinate records.
- Supports organizational reporting structures.
- Works together with OWD.

Example:

Principal
→ HOD
→ Faculty
→ Students

---

## What are Sharing Rules?

Sharing Rules provide automatic exceptions to OWD settings.

They allow administrators to share records with groups of users who normally would not have access.

Types:
1. Owner-Based Sharing Rules
2. Criteria-Based Sharing Rules

Benefits:
- Extends record access.
- Supports collaboration.
- Reduces manual sharing.

---

## Difference Between Profile, Permission Set, and Role

| Feature | Profile | Permission Set | Role |
|----------|----------|---------------|------|
| Purpose | Defines what a user can do | Grants additional permissions | Defines record visibility |
| Assignment | One per user | Multiple per user | One per user |
| Controls | Object, Field, App permissions | Extra permissions | Record access |
| Mandatory | Yes | No | No |
| Access Type | Functional Access | Additional Functional Access | Record-Level Access |

---

## College Security Design

### Users
- Student
- Faculty
- Placement Officer
- HOD
- Principal
- Salesforce Administrator

### Access Design

| Role | View Student Records | View Faculty Records | View Placement Records | Edit Attendance | Edit Placement Data | Edit Student Details | Delete Records |
|--------|--------------------|---------------------|-----------------------|----------------|-------------------|-------------------|---------------|
| Student | Own Only | No | No | No | No | Own Only | No |
| Faculty | Department Students | Yes | No | Yes | No | Limited | No |
| Placement Officer | Yes | No | Yes | No | Yes | No | No |
| HOD | Department Records | Yes | Yes | Yes | Yes | Yes | No |
| Principal | All Records | All Records | All Records | Yes | Yes | Yes | No |
| Salesforce Administrator | Full Access | Full Access | Full Access | Yes | Yes | Yes | Yes |

### Security Controls

- OWD = Private
- Role Hierarchy used for management access.
- Sharing Rules used for department-level visibility.
- Permission Sets used for additional access.

---

## Faculty Access Scenario

### Requirement

- Faculty A should only see CSE students.
- Faculty B should only see ECE students.
- HOD should see all students within the department.
- Principal should see everything.

### OWD

Student Records = Private

### Role Hierarchy

Principal
→ HOD
→ Faculty

### Sharing Rules

- Share CSE student records with Faculty A.
- Share ECE student records with Faculty B.
- Share department records with HOD.

### Permission Sets

Faculty Permission Set:
- Read Student Records
- Update Attendance

HOD Permission Set:
- Read/Edit Department Records

Principal Permission Set:
- Full Read Access

### Why This Design?

- Protects student privacy.
- Ensures department-specific visibility.
- Prevents unauthorized modifications.
- Supports organizational hierarchy.

---

## Reflection: Why is Record-Level Security Important?

1. Protects sensitive student information.
2. Prevents unauthorized access.
3. Ensures data privacy.
4. Supports compliance requirements.
5. Reduces accidental modifications.
6. Maintains data integrity.
7. Restricts access based on job responsibilities.
8. Supports organizational hierarchy.
9. Improves system security.
10. Prevents misuse of institutional data.
11. Enables controlled collaboration.
12. Ensures only authorized users can edit records.

Record-level security is essential because not every user should have access to every record. It protects data, improves privacy, and ensures users only access information required for their responsibilities.
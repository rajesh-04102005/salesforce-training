# Day 9 - LWC Communication

## Component Communication

Lightning Web Components communicate with each other to share data and trigger actions inside applications.

### Types of Communication

### 1. Parent to Child

* Uses `@api`
* Parent sends data to child component
* Parent can call child methods

Example:

```js
@api counter;
```

### 2. Child to Parent

* Uses Custom Events
* Child dispatches events
* Parent listens to events

Example:

```js
this.dispatchEvent(new CustomEvent('add'));
```

### 3. Unrelated Components

* Uses Lightning Message Service (LMS)
* Components communicate without parent-child relation

---

# Dashboard Design

## Student Dashboard

Components:

* Student Profile
* Attendance
* Courses
* Notifications

Communication:

* Attendance component updates dashboard
* Notification component alerts students
* Course component sends updates to profile

---

## Faculty Dashboard

Components:

* Student List
* Marks Upload
* Attendance Manager
* Notifications

Communication:

* Marks Upload updates Student List
* Attendance Manager sends attendance updates
* Notifications alert faculty actions

---

## Admin Dashboard

Components:

* User Management
* Course Allocation
* Reports
* System Notifications

Communication:

* User Management updates reports
* Course Allocation updates student and faculty modules
* Notifications broadcast system messages

---

# Data Flow Explanation

## Process: Student Registration

### Flow

UI →
Validation →
Flow →
Apex →
Database →
Notification

### Explanation

1. User enters registration details in UI.
2. Validation checks required fields and formats.
3. Salesforce Flow processes automation logic.
4. Apex handles backend business logic.
5. Data is stored in Salesforce Database.
6. Notification is sent to student and admin.

This architecture keeps frontend and backend separated.

---

# Aura vs LWC

| Aura Components   | Lightning Web Components |
| ----------------- | ------------------------ |
| Older framework   | Modern framework         |
| Less performance  | Faster performance       |
| Complex syntax    | Simple JavaScript        |
| Heavy framework   | Lightweight              |
| Event complexity  | Better communication     |
| Slower rendering  | Faster rendering         |
| Proprietary model | Web standards based      |

## Why Salesforce Moved to LWC

Salesforce moved to LWC because:

* Better performance
* Faster rendering
* Modern web standards
* Improved developer experience
* Reusable modular architecture
* Better scalability

---

# Reflection

## Why Enterprise Applications Need Modular Architecture

Enterprise applications are large and complex. Modular architecture helps divide systems into reusable components.

Benefits:

* Easier maintenance
* Better scalability
* Reusable code
* Faster development
* Independent testing
* Easier debugging

Modular systems reduce dependency between components and improve application stability.

---
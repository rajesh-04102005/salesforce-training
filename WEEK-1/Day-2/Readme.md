# Day 2 - Salesforce Platform Basics

## What is Salesforce Platform?

Salesforce Platform is a cloud-based platform that helps businesses manage customer relationships, automate processes, and build custom applications without managing servers or infrastructure.

It provides:
- CRM functionality
- Data storage using Objects
- User interface using Apps and Tabs
- Automation tools
- Development tools like Apex and APIs

Salesforce follows a multi-tenant architecture where multiple organizations share the same infrastructure securely.

---

# Salesforce Core Concepts

## 1. What is an App?

An App in Salesforce is a collection of related tabs, objects, and tools grouped together for a specific business purpose.

### Examples:
- Sales App
- Service App
- College Management App

### Purpose:
- Organizes functionality
- Improves navigation
- Helps users work efficiently

---

## 2. What is an Object?

An Object in Salesforce is similar to a database table used to store data.

Objects contain:
- Fields (columns)
- Records (rows)

### Standard Objects:
- Account
- Contact
- Opportunity
- Lead

### Custom Objects:
- Student
- Faculty
- Course

---

## 3. What is a Tab?

A Tab is the user interface entry point used to access objects and records.

### Examples:
- Accounts Tab
- Contacts Tab
- Students Tab

Tabs help users navigate the application easily.

---

# Relationship Between App, Object, and Tab

```text
App
 ├── Tabs
 │     ├── Objects
 │     │      ├── Records
```

Example:

```text
College Management App
 ├── Students Tab
 ├── Faculty Tab
 ├── Courses Tab
```

---

# Configuration vs Coding

## Configuration

Configuration means customizing Salesforce using no-code or low-code tools.

### Tools:
- Flow Builder
- Validation Rules
- Page Layouts
- Object Manager

### Examples:
1. Creating a custom object
2. Automating approval workflows

### Advantages:
- Faster development
- Easier maintenance
- No programming required

---

## Coding

Coding means developing advanced functionality using programming languages and frameworks.

### Technologies:
- Apex
- Lightning Web Components (LWC)
- APIs
- SOQL

### Examples:
1. Payment gateway integration
2. Complex approval logic using Apex

### Advantages:
- More flexibility
- Advanced business logic
- Better customization

---

# Difference Between Configuration and Coding

| Configuration | Coding |
|---|---|
| No-code/low-code | Requires programming |
| Faster implementation | More flexible |
| Easier to maintain | Handles complex logic |
| Used by Admins | Used by Developers |

---

# System Design

## System Name:
College Management System

## App Name:
College Management App

---

# Objects in the App

| Object | Purpose |
|---|---|
| Student | Stores student information |
| Faculty | Stores faculty details |
| Course | Stores course information |
| Attendance | Tracks attendance |
| Examination | Stores exam results |
| Fee | Tracks fee payments |

---

# User Interaction

## Admin
- Manages students and faculty
- Creates courses
- Generates reports

## Faculty
- Marks attendance
- Updates marks
- Manages student performance

## Students
- View attendance
- Check exam results
- Access course information

---

# Example App Structure

```text
College Management App
 ├── Students Tab
 ├── Faculty Tab
 ├── Courses Tab
 ├── Attendance Tab
 ├── Examination Tab
 └── Fee Tab
```

---

# CRM Concepts in Salesforce

| CRM Concept | Salesforce Object |
|---|---|
| Account | Standard Object |
| Contact | Standard Object |
| Opportunity | Standard Object |
| Lead | Standard Object |

---

# Multi-Tenant Architecture

Salesforce uses multi-tenant architecture.

This means:
- Multiple organizations share the same infrastructure
- Data remains secure and isolated
- Updates happen automatically

### Benefits:
- Scalability
- Lower infrastructure cost
- Automatic upgrades
- High availability

---

# How Developers Extend Salesforce

Developers extend Salesforce using:
- Apex programming
- Lightning Components
- APIs
- Integrations
- AppExchange apps

Examples:
- External system integration
- Advanced automation
- Custom dashboards

---

# Trailhead Modules Completed

## Agentforce 360 Platform Basics
Completed Topics:
- Platform overview
- Salesforce architecture
- Navigation
- Setup
- AppExchange

---

## Agentforce 360 Platform Development Basics
Completed Topics:
- No-code development
- Coding overview
- Apex basics
- Platform extension

---

# Key Learnings

- Salesforce is a cloud-based CRM platform
- Apps organize business functionality
- Objects store data
- Tabs help users navigate
- Configuration is used for simple customization
- Coding is used for advanced logic
- Salesforce uses multi-tenant architecture
- Developers extend Salesforce using Apex and APIs

---
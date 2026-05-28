# Day 10 Mini Project – College Management System

## System Overview

The College Management System is a mini CRM-based Salesforce application designed to manage students, faculty, departments, and courses within a college environment.

The system integrates:

* CRM concepts
* Data modeling
* Validation rules
* Flow automation
* Apex logic
* Lightning Web Components (LWC)
* Triggers and event-driven behavior

The application allows students to register for courses, faculty to manage attendance, and administrators to automate academic processes.

---

# CRM Concepts

The system uses CRM concepts to organize and manage academic data.

### Main CRM Entities

* Student
* Faculty
* Course
* Department

### CRM Usage

* Store student information
* Track course registrations
* Manage faculty assignments
* Maintain department records
* Monitor attendance and notifications

---

# Data Model

## Objects Used

### Student__c

Fields:

* Name
* Email
* Attendance Percentage
* Department

### Faculty__c

Fields:

* Name
* Email
* Assigned Courses

### Course__c

Fields:

* Course Name
* Seats Available
* Maximum Seats
* Faculty Lookup

### Department__c

Fields:

* Department Name
* HOD

### Registration__c

Fields:

* Student Lookup
* Course Lookup
* Registration Date

---

# Validation Rules

Validation rules ensure data accuracy and consistency.

## Examples

### Email Mandatory

Ensures every student record contains an email.

### Seat Limit Validation

Prevents registrations when seats exceed the maximum limit.

### Attendance Validation

Attendance percentage cannot be greater than 100.

---

# Flows

Salesforce Flows automate business processes.

## Implemented Flows

### Registration Confirmation Flow

* Sends confirmation after successful registration.

### Attendance Warning Flow

* Sends warning notifications for low attendance.

### Faculty Notification Flow

* Alerts faculty when a course becomes full.

---

# Apex Logic

Apex is used for advanced business logic.

## Features

### Eligibility Calculation

Checks whether students meet eligibility criteria for course registration.

### Bulk Registration Handling

Processes multiple student registrations efficiently.

### Trigger Logic

* Automatically updates remaining seats
* Generates alerts when limits are reached

---

# UI Screens

## Student Dashboard

Features:

* View courses
* Register for subjects
* Check attendance

## Faculty Dashboard

Features:

* Manage courses
* View enrolled students
* Track attendance

## Registration Screen

Features:

* Course selection
* Validation checks
* Real-time seat availability

---

# Complete Data Flow

Student clicks Register
↓
LWC Registration Screen
↓
Validation Rules check input
↓
Flow automation starts
↓
Apex logic processes registration
↓
Trigger updates seat count
↓
Database stores registration
↓
Notification email sent to student and faculty

---

# Reflection

This project helped me understand how enterprise applications integrate frontend UI, backend logic, databases, automation, and event-driven systems together.

I learned:

* Why modular architecture is important
* How CRM systems organize business data
* How Salesforce automates workflows
* Why Apex is needed for advanced logic
* How LWC improves user interaction
* How enterprise systems scale using reusable components

This mini project provided practical understanding of real-world Salesforce application architecture.

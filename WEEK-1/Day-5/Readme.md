# Day 5 - Apex Introduction

## What is Apex?
Apex is a programming language developed by Salesforce. It is used to add custom business logic and automation inside Salesforce applications.

---

## Difference Between Flow and Apex

| Flow | Apex |
|------|------|
| No-code/low-code | Programming language |
| Easy to build | Requires coding knowledge |
| Best for simple automation | Best for complex logic |
| Faster development | More flexible and powerful |

---

## Configuration vs Coding

| Configuration | Coding |
|---------------|--------|
| Uses clicks and setup | Uses Apex code |
| Easy to maintain | More customizable |
| Limited flexibility | Handles advanced logic |

---

## Real Examples Where Apex Is Needed

1. Complex fee calculation system
2. Integration with external payment gateway
3. Advanced student eligibility checking

---

## College Management System Design

### CRM
Used to manage students, courses, faculty, and admissions.

### Objects
- Student
- Course
- Faculty

### Relationships
- Student ↔ Course
- Faculty ↔ Course

### Validation
- Email field required
- Phone number validation

### Flow
- Auto email notification after registration

### Apex
- Custom admission eligibility logic

---

## Pseudocode Examples

### Example 1
IF seats are full  
THEN block registration

### Example 2
IF attendance < 75%  
THEN notify student

---

## Reflection

Enterprise systems eventually need programming because business requirements become complex and cannot always be handled using only clicks and configuration.
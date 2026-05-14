# Day 3 Learning Notes

## What I Learned

Today I learned how Salesforce stores and manages business data using structured objects and relationships.

---

# Key Concepts Learned

## 1. Objects
Objects are database tables used to store information.

Example:
- Student
- Course
- Department

---

## 2. Fields
Fields store specific pieces of information.

Example:
- Student Name
- Age
- Email

---

## 3. Records
Records are individual entries inside objects.

Example:
Student Name = Raj

---

## 4. Relationships
Relationships connect objects together.

Example:
- One Department can have many Students.
- One Course can have many Students.

---

# Relationship Types Learned

## Lookup Relationship
Loose connection between objects.

## Master-Detail Relationship
Strong parent-child relationship.

---

# Schema Builder

Schema Builder is a visual tool used to:
- Create objects
- Create fields
- Design relationships
- Visualize data models

---

# Formula Fields

Formula Fields automatically calculate values.

Examples:
- Full Name
- Percentage
- Remaining Seats

Benefits:
- Automation
- Reduced manual work
- Accurate calculations

---

# Validation Rules

Validation Rules prevent invalid data from being saved.

Examples:
- Age cannot be negative
- Email cannot be blank
- Seats cannot exceed limit

Benefits:
- Better data quality
- Prevents incorrect entries

---

# Real Understanding

I understood that Salesforce is called a metadata-driven platform because:
- Most configurations are done without coding.
- Objects, fields, validations, and relationships are created using metadata.

---

# Final Understanding

Enterprise systems require:
- Structured data
- Relationships
- Validation
- Automation

instead of random spreadsheets.
# Salesforce Summer Program - Day 3

## Topics Covered
- Objects
- Fields
- Records
- Relationships
- Schema Builder
- Formula Fields
- Validation Rules
- Structured Enterprise Data

---

# 1. Difference Between App, Object, Record, and Field

| Term | Meaning | Example |
|------|----------|----------|
| App | Collection of related objects, tabs, and tools | Sales App |
| Object | Database table that stores data | Student Object |
| Record | Single row of data inside an object | Student: Raj |
| Field | Column that stores specific information | Student Name |

---

# 2. Standard vs Custom Objects

## Standard Objects
Objects already provided by Salesforce.

### Examples
- Account
- Contact
- Opportunity
- Lead

---

## Custom Objects
Objects created based on business requirements.

### Examples
- Student__c
- Faculty__c
- Course__c
- Department__c

Custom objects end with:
```text
__c
```

---

# 3. College Data Model

## Objects

1. Student
2. Faculty
3. Course
4. Department

---

## Relationships

| Parent Object | Child Object | Relationship Type |
|----------------|---------------|-------------------|
| Department | Student | Lookup |
| Department | Faculty | Lookup |
| Department | Course | Master-Detail |
| Course | Student | Lookup |

---

## Data Model Diagram

```text
Department
   │
   ├── Faculty
   │
   ├── Course
   │      │
   │      └── Student
   │
   └── Student
```

---

# 4. Formula Fields

## Formula Field 1: Full Name

### Formula
```text
First_Name__c & " " & Last_Name__c
```

### Purpose
Automatically combines first name and last name.

### Why Use It?
Prevents users from manually typing full names repeatedly.

---

## Formula Field 2: Remaining Seats

### Formula
```text
Total_Seats__c - Filled_Seats__c
```

### Purpose
Shows available seats in a course.

### Why Use It?
Automatically updates when students enroll.

---

## Formula Field 3: Percentage

### Formula
```text
(Obtained_Marks__c / Total_Marks__c) * 100
```

### Purpose
Calculates student percentage automatically.

### Why Use It?
Avoids manual calculation errors.

---

# 5. Validation Rules

## Validation Rule 1: Email Cannot Be Empty

### Formula
```text
ISBLANK(Email__c)
```

### Error Message
Email cannot be empty.

### Why?
Prevents missing contact information.

---

## Validation Rule 2: Student Age Cannot Be Negative

### Formula
```text
Student_Age__c < 0
```

### Error Message
Student age cannot be negative.

### Why?
Prevents invalid age values.

---

## Validation Rule 3: Course Seats Cannot Exceed Limit

### Formula
```text
Filled_Seats__c > Total_Seats__c
```

### Error Message
Filled seats cannot exceed total seats.

### Why?
Prevents overbooking.

---

# 6. Reflection

## Why Structured Enterprise Data Matters

Companies cannot manage large systems efficiently using random spreadsheets because:

- Data becomes inconsistent
- Duplicate records appear
- Relationships are difficult to maintain
- Reporting becomes complicated
- Multiple users may overwrite data
- Security and validation become difficult

Salesforce solves these problems using:
- Objects
- Relationships
- Validation Rules
- Formula Fields
- Automation
- Centralized data storage

Structured enterprise data improves:
- Accuracy
- Scalability
- Reporting
- Security
- Productivity

---

# Conclusion

This project helped me understand:
- Salesforce data modeling
- Relationships between objects
- Formula Fields
- Validation Rules
- Why enterprise systems need structured data
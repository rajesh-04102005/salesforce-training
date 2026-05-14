# Day 3 Tasks

## Task 1: Design a College Management System

### Objects Created
- Student
- Faculty
- Course
- Department

---

## Relationships

| Parent | Child | Type |
|--------|--------|------|
| Department | Student | Lookup |
| Department | Faculty | Lookup |
| Department | Course | Master-Detail |
| Course | Student | Lookup |

---

# Task 2: Formula Field Thinking

## Formula 1: Full Name

```text
First_Name__c & " " & Last_Name__c
```

### Why?
Automatically combines names.

---

## Formula 2: Remaining Seats

```text
Total_Seats__c - Filled_Seats__c
```

### Why?
Shows live seat availability.

---

## Formula 3: Percentage

```text
(Obtained_Marks__c / Total_Marks__c) * 100
```

### Why?
Avoids manual calculations.

---

# Task 3: Validation Rule Thinking

## Validation Rule 1: Email Cannot Be Empty

```text
ISBLANK(Email__c)
```

### Problem Prevented
Missing contact information.

---

## Validation Rule 2: Student Age Cannot Be Negative

```text
Student_Age__c < 0
```

### Problem Prevented
Invalid age values.

---

## Validation Rule 3: Course Seats Cannot Exceed Limit

```text
Filled_Seats__c > Total_Seats__c
```

### Problem Prevented
Overbooking of courses.

---

# Task 4: Reflection

## Why Companies Need Structured Data

Structured data is important because:
- It reduces duplication
- Improves reporting
- Maintains relationships
- Supports automation
- Increases security

Random spreadsheets are difficult to maintain in large organizations.


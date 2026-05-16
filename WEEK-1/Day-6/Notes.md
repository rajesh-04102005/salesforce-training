# Notes – Day 6

## SOQL
- Salesforce Object Query Language
- Used to retrieve data from Salesforce objects

Example:
SELECT Name FROM Account

---

## SOSL
- Salesforce Object Search Language
- Used for searching across multiple objects

---

## Apex Triggers
- Code that runs automatically on record events
- Events:
  - before insert
  - before update
  - after insert
  - after update
  - delete

---

## Before Trigger
- Runs before saving records
- Used for validation and updating fields

## After Trigger
- Runs after saving records
- Used for related records and notifications

---

## Flow vs Trigger

Flow:
- No-code automation
- Simple logic

Trigger:
- Code-based automation
- Complex logic and bulk processing
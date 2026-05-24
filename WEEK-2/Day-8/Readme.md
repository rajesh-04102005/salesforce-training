# Day 8 - Lightning Web Components (LWC) Basics

## What is LWC?

Lightning Web Components (LWC) is Salesforce’s modern UI framework used to build fast, reusable, and scalable components using standard web technologies.

LWC is based on:
- HTML
- JavaScript
- CSS
- Web Components Standards

It helps developers create responsive and efficient applications inside Salesforce.

---

# Why Salesforce Uses LWC

Salesforce introduced LWC to improve:
- Performance
- Developer productivity
- Reusability
- Maintainability

## Advantages of LWC

- Faster rendering using native browser features
- Modern JavaScript support (ES6+)
- Reusable components
- Easy integration with Salesforce data
- Better performance than Aura Components
- Cleaner and simpler code structure

---

# UI Screens

## Bike Card Component
Displays:
- Bike Name
- Description
- Price
- Category
- Material
- Bike Image

## Bike Selection App
Displays:
- Available Bikes
- Current logged-in username
- Dynamic bike details
- Interactive bike selection

---

# Component Breakdown

## bikeCard Component
Purpose:
- Displays a single bike card with details.

Files:
- bikeCard.html
- bikeCard.js
- bikeCard.js-meta.xml

---

## selector Component
Purpose:
- Handles bike selection events.
- Displays logged-in user name using @wire.

Files:
- selector.html
- selector.js
- selector.js-meta.xml

---

## detail Component
Purpose:
- Displays selected bike information dynamically.

Files:
- detail.html
- detail.js
- detail.css

---

## list Component
Purpose:
- Displays available bike list.

---

## tile Component
Purpose:
- Represents individual bike items.

---

# Frontend vs Backend Logic

## Frontend Logic

Handled using:
- HTML templates
- CSS styling
- JavaScript event handling

Examples:
- Bike selection
- UI rendering
- Dynamic updates
- SLDS styling

---

## Backend Logic

Handled using:
- Salesforce Wire Service
- Lightning Data Service
- Apex (when required)

Examples:
- Fetching current user name
- Accessing Salesforce records
- CRUD operations

---

# Reflection

Through this project, I learned:
- Basics of Lightning Web Components
- Component-based architecture
- Parent-child communication
- Event handling using CustomEvent
- Wire service and Salesforce data integration
- Component deployment using Salesforce CLI
- Lightning App Builder integration

This project improved my understanding of modern Salesforce frontend development and practical LWC implementation.
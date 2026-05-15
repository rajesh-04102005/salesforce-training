# Salesforce Summer Program – Day 4
# Flow Builder and Business Process Automation

---

## 1. What is Flow Builder?

Flow Builder is a declarative automation tool in :contentReference[oaicite:0]{index=0} that helps admins and developers automate business processes without writing code.

Using Flow Builder, organizations can:
- Automate repetitive tasks
- Reduce manual effort
- Improve workflow efficiency
- Minimize human errors
- Create guided user experiences

Flow Builder is one of the most powerful automation tools available in Salesforce because it allows businesses to build logic visually using drag-and-drop components.

---

# 2. Types of Flows

## A. Screen Flow

A Screen Flow is an interactive flow that collects input from users through screens.

### Features
- Displays forms and questions
- Accepts user input
- Guides users step-by-step
- Can create or update records

### Example
A student registration form where students enter:
- Name
- Email
- Course
- Phone Number

After submission:
- A student record is created
- A confirmation message is shown

### Use Cases
- Admission Forms
- Employee Onboarding
- Survey Forms
- Help Desk Requests

---

## B. Record-Triggered Flow

A Record-Triggered Flow runs automatically when a record is:
- Created
- Updated
- Deleted

No user interaction is required.

### Features
- Fully automated
- Runs in the background
- Responds instantly to record changes
- Can update related records

### Example
When a student registers for a course:
- Remaining seats are automatically reduced
- Faculty receives notification if seats are full

### Use Cases
- Auto Email Notifications
- Approval Processes
- Auto Status Updates
- Task Creation

---

# 3. Automation Ideas

## 1. Auto Email After Registration
When a student registers successfully:
- Salesforce automatically sends a confirmation email.

### Benefits
- Instant communication
- Better user experience
- Reduced manual follow-up

---

## 2. Auto Update Remaining Seats
Whenever a student enrolls:
- Available seats in the course are automatically reduced.

### Benefits
- Real-time tracking
- Prevents overbooking

---

## 3. Notify Faculty When Course is Full
If available seats become zero:
- Faculty receives an automatic notification email.

### Benefits
- Faster decision making
- Better course management

---

## 4. Generate Student ID Automatically
When a new student record is created:
- Salesforce generates a unique Student ID.

### Example
STU-1001  
STU-1002

### Benefits
- Removes manual work
- Avoids duplicate IDs

---

## 5. Send Fee Deadline Reminder
Before fee due dates:
- Automated reminder emails are sent to students.

### Benefits
- Improves payment completion
- Reduces manual reminders

---

# 4. Flow Diagram

## Student Registration Automation Flow

```text
[Student Submits Form]
            ↓
[Create Student Record]
            ↓
[Generate Student ID]
            ↓
[Update Remaining Seats]
            ↓
[Check Seat Availability]
        ↓           ↓
      Yes            No
      ↓              ↓
[Send Confirmation] [Notify Faculty]
      ↓
[Send Fee Reminder]

---

# 5. Manual vs Automated Process

| Manual Process | Automated Process |
|---|---|
| Staff enters data manually | Flow creates records automatically |
| Emails are sent manually | Automatic email notifications |
| Seat count is updated manually | Seats are updated instantly |
| More chances of human errors | Higher accuracy and consistency |
| Time-consuming process | Faster execution |
| Requires more manpower | Saves time and effort |

### Example

#### Manual Process
1. Student submits registration form  
2. Staff verifies details manually  
3. Staff sends confirmation email  
4. Staff updates course seat count  
5. Faculty is informed manually  

#### Automated Process
1. Student submits registration form  
2. Salesforce Flow creates student record automatically  
3. Confirmation email is sent instantly  
4. Remaining seats are updated automatically  
5. Faculty receives automatic notification if course is full  

---

# 6. Reflection – Why Automation Matters in Enterprise Systems

Automation plays a major role in modern enterprise systems because organizations manage large amounts of data and repetitive tasks every day.

Using automation:
- Increases productivity
- Reduces manual work
- Minimizes human errors
- Saves time and operational cost
- Improves customer experience
- Ensures process consistency

In Salesforce, Flow Builder allows businesses to automate workflows without coding. This helps organizations build efficient systems that are scalable, reliable, and easy to maintain.

### My Learning Reflection

From this activity, I learned:
- How Flow Builder simplifies automation
- The difference between Screen Flows and Record-Triggered Flows
- How automation improves enterprise workflows
- The importance of reducing manual tasks in business systems

Automation is essential for creating smart, fast, and reliable enterprise applications.
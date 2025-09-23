Phase 1: https://docs.google.com/document/d/11xv7b0wglcisC8SG9CRtLvgFJnjsmDp7XtXTQwlLS-I/edit?tab=t.0
Phase 2: https://docs.google.com/document/d/1Qen0nPHXFKOGEQZMv68e0Hq2hLArXDHOyeICmb2i3U4/edit?tab=t.0
Phase 3: https://docs.google.com/document/d/1uaxA6Q-4-kA0SHXxKzOZOEfZZ41c-3UyWVYF9LHN7Xw/edit?tab=t.0
Phase 4: https://docs.google.com/document/d/1h-ejkHKer_wZ25SBCGe-jKKq55pHCIhP6bC8soqGAoI/edit?tab=t.0
Phase 5:
Phase 6:
Phase 7:
Phase 8:
Phase 9:
Phase 10:
# 🎓 Campus Event Management System  

---

## 🏫 Industry  
Education / Student Communities  

---

## 📌 Project Type  
B2C Salesforce CRM Implementation  

---

## 🎯 Target Users  
- **Students** → Register for events, provide feedback.  
- **Organizers** → Manage events, monitor attendance.  
- **Faculty/Staff** → Oversee workshops, seminars, and cultural fests.  
- **Admins/Managers** → Track event success, participation trends, and student engagement.  

---

## ❗ Problem Statement  
Colleges often struggle to manage campus events effectively:  
- Event details are scattered across posters, emails, and WhatsApp groups.  
- Student registrations are tracked manually via spreadsheets or Google Forms.  
- Attendance tracking is inconsistent.  
- Feedback collection is irregular and unstructured.  

The institute needs a **Salesforce CRM-based solution** to:  
- Centralize event management.  
- Automate student registrations & confirmations.  
- Track attendance and feedback.  
- Provide dashboards to analyze participation and event success.  

---

## 🎯 Business Goals  
1. **Centralize Event Management**  
   - Store all event details in one place.  
   - Provide organizers with easy event setup and monitoring.  

2. **Automate Student Registrations**  
   - Online registrations with automatic confirmation emails.  
   - Track event capacity and attendance in real time.  

3. **Attendance & Feedback Tracking**  
   - Record attendance directly in Salesforce.  
   - Collect structured feedback after events.  

4. **Analytics & Reporting**  
   - Dashboards for event popularity, attendance trends, and feedback analysis.  
   - Enable data-driven decision-making for future events.  

---

## ⭐ Key Features  

| Feature                  | Description                                                                 |
|---------------------------|-----------------------------------------------------------------------------|
| **Event Management**      | Create, store, and manage campus events with details like type, date, and venue. |
| **Student Registration**  | Allow students to register online with automated confirmation emails.       |
| **Attendance Tracking**   | Mark attendance in Salesforce for each event.                              |
| **Feedback Collection**   | Gather structured feedback linked to specific events.                      |
| **Analytics Dashboard**   | Reports on participation, event popularity, and feedback trends.            |

---

## 📌 Detailed Use Cases  

### 1. Event Creation  
- **Actor:** Organizer  
- **Flow:** Organizer creates an event in Salesforce with name, type, date, and location.  

### 2. Student Registration  
- **Actor:** Student, Organizer  
- **Flow:** Student registers → Salesforce auto-creates a **Registration record** → Confirmation email sent.  

### 3. Attendance Tracking  
- **Actor:** Organizer  
- **Flow:** During the event, attendance is marked for registered students.  

### 4. Feedback Collection  
- **Actor:** Student  
- **Flow:** After the event, students provide ratings and comments stored in Salesforce.  

### 5. Analytics & Reporting  
- **Actor:** Admin/Manager  
- **Flow:** Dashboards show event popularity, student participation, and feedback summaries.  

---

## 🗂 Data Model  

| Object            | Key Fields                                                |
|-------------------|----------------------------------------------------------|
| **Event**         | Name, Date, Type (Workshop, Cultural, Seminar), Location |
| **Student**       | Name, Email, Phone, Department, Year                     |
| **Registration**  | Student, Event, Registration Date, Attendance, Feedback  |

---

## 👨‍💻 Author  
**Shaik Raqueebul Islam (RAQUEE07)**  
- Salesforce Enthusiast | Cloud & CRM Developer  
- GitHub: [RAQUEE07](https://github.com/RAQUEE07)  

---
# Campus Event Management App

## Phase 2: Salesforce Setup

In Phase 2, we configured the Campus Event Management App in Salesforce Lightning. The following tasks were completed:

### 1. App Creation
- **App Name:** Campus Event Management App
- **Developer Name:** Campus_Event_Management_App
- **Branding:** Primary color #0070D2
- Added navigation items for easy access:
  - Event Details
  - Participants
  - Feedback
  - Sponsors
  - Calendar
  - Reports
  - Dashboards

### 2. Custom Objects & Fields
**Custom objects created:**
- **Event Details**
- **Participants**
- **Feedback** (optional)
- **Sponsors** (optional)

**Sample fields for Event Details:**
- Event Name (Text)
- Event_Date (Date)
- Event_Type (Picklist)
- Location (Text)
- Number of Participants (Number)

**Sample fields for Participants:**
- Participant Name (Text)
- Email (Email)
- Contact Number (Phone)
- Event Registered (Lookup to Event Details)
- Registration Date (Date)

**Feedback object sample fields:**
- Feedback Name (Text)
- Event (Lookup)
- Participant (Lookup)
- Rating (Number)
- Comments (Long Text Area)

**Sponsors object sample fields:**
- Sponsor Name (Text)
- Contact Person (Text)
- Email (Email)
- Phone (Phone)
- Sponsored Event (Lookup to Event Details)

### 3. Tabs & Navigation
- Tabs created for all custom objects
- Tabs added to app navigation for easy access via the App Launcher

### 4. Field-Level Security
- All fields set to **Visible** for relevant profiles
- Editable for Admin, Sales, Marketing profiles
- Lookup relationships verified

### 5. Testing & Verification
- Sample records created for each object
- Lookup relationships confirmed
- Navigation, search, and related lists verified
- Picklist, date, and number fields tested

### 6. Documentation
All screenshots and Phase 2 setup documentation are uploaded to the repository in the following folder:





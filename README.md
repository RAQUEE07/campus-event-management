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

## Phase 1: Problem Understanding & Industry Analysis

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
## ⚙️ Phase 2: Org Setup & Configuration

## 1. Salesforce Edition
- **Edition Used:** Developer Edition  
- **Purpose:** Free, all-in-one environment for building and testing the Campus Event Management App.

---

## 2. Company Profile Setup
- **Configured:** Default time zone, default currency  
- **Use Case:** Ensures consistency across event operations.

---

## 3. Business Hours & Holidays
- **Status:** Acknowledged as important for scheduling and calculations.  
- **Note:** Not configured in this project’s scope.

---

## 4. Fiscal Year Settings
- **Type:** Standard Fiscal Year (January – December).  
- **Reason:** Simplifies financial alignment for event cycles.

---

## 5. User Setup & Licenses
- **Created Users:**  
  - Organizer  
  - Participant  
- **Assigned License:** Salesforce (full CRM access).

---

## 6. Profiles
- **Action:** Cloned **Standard User** → Created custom **Event Organizer** profile.  
- **Assignment:** Organizer test user.

---

## 7. Roles
- **Decision:** Role hierarchy **not configured**.  
- **Reason:** Relied on ownership & profile-based security.

---

## 8. Permission Sets
- **API Callout Access:** Granted permissions needed for integrations.  
- **Event Management App Access:** Granted visibility to custom tabs and objects, bypassing profile limitations.

---

## 9. Organization-Wide Defaults (OWD)
- **Event_Details__c:** Private  
- **Participant__c:** Private  
- **Purpose:** Protect sensitive event and participant data.

---

## 10. Deployment Basics
- **Tool:** Salesforce DX (SFDX).  
- **Process:** Retrieved and deployed components using **package.xml** manifest.

---


### App Creation
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

### Custom Objects & Fields
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

## 🗂 Phase 3: Data Modeling & Relationships

## 1. Dashboard After Login
- **Action:** Logged into Salesforce Developer Edition.  
- **Access:** App Launcher, Setup, and other Salesforce tools available.

---

## 2. App Creation
- **App Name:** *Campus Event Management App*  
- **Branding:** Primary color `#0070D2`  
- **Navigation Items Added:** Event Details, Participants, Feedback, Sponsors, Reports, Dashboards.

---

## 3. Standard & Custom Objects
- **Custom Objects:**  
  - **Event_Details__c** → Stores event details.  
  - **Participant__c** → Tracks registered participants.  
  - **Feedback__c** (optional) → Captures participant feedback.  
  - **Sponsor__c** (optional) → Stores sponsor details.  

- **Standard Objects:**  
  - **User** → Used via lookup to assign ownership (e.g., Event Organizer).

---

## 4. Custom Fields
- **Event_Details__c:** `Event_Date__c (Date)`, `Event_Type__c (Picklist)`.  
- **Participant__c:** `Participant_Email__c (Email, Unique)`.  
- **Sponsor__c:** `Sponsor_Name__c (Text)`.  
- **Feedback__c:** `Feedback_Rating__c (Number, 1–5)`.  
- **Relationships:**  
  - `Event__c (Lookup → Event_Details__c)` on `Participant__c`.  
  - `Participant__c (Lookup → Participant__c)` on `Feedback__c`.

---

## 5. Record Types
- **Decision:** Not used.  
- **Reason:** Kept a single streamlined process for all event types.

---

## 6. Page Layouts
- **Event_Details__c:** Related lists for Participants & Sponsors.  
- **Participant__c:** Related list for Feedback.  
- **Sponsor__c:** Lookup to Event_Details__c.  
- **Feedback__c:** Lookup to Participant__c.

---

## 7. Relationships
- **Lookup:** Feedback → Participant (feedback can exist independently).  
- **Master-Detail:** Participant → Event Details (participants must belong to an event).  
- **Hierarchical:** Not used (only for User object).

---

## 8. Junction Objects
- **Participant__c:** Acts as a semi-junction object linking `Event_Details__c` & `Feedback__c`.  
- **Benefit:** Allows multiple participants per event and multiple feedback entries per participant.

---

## 9. Tabs Creation
- Created tabs for all custom objects to make them accessible in the navigation bar.

---

## 10. Navigation Items
- Added: Event Details, Participants, Feedback, Sponsors, Reports, Dashboards.

---

## 11. Accessing the App
- Accessed via App Launcher.  
- All configured objects and navigation items visible.

---

## 12. Testing Custom Objects
- **Sample Records Created:**  
  - Event (e.g., Campus Tech Seminar).  
  - Participant linked to the Event.  
  - Feedback linked to Participant & Event.  
  - Sponsor linked to Event.

---

## 13. Verification of Functionality
- Tabs open correctly.  
- Records searchable.  
- Related lists display linked records.  
- Picklists, text, date, and number fields validated.

---

## ⚡ Phase 4: Automation & Approvals

## 1. Workflow Rules
- **Object:** Participant__c  
- **Rule:** Triggered when a new Participant record is created.  
- **Action:** Sends email alert to organizer confirming participant registration.  
- **Outcome:** Automates notifications without manual intervention.  

---

## 2. Email Alerts
- **Alert Name:** Participant_Approval_Reminder  
- **Object:** Participant__c  
- **Template Used:** Standard *Appointment Confirmation* template (customized for events).  
- **Recipients:** Organizer, Integration User, and specific test users.  
- **From Address:** Current User’s email address.  

---

## 3. Field Updates
- **Field Update Name:** Set_Status_Approved  
- **Object:** Participant__c  
- **Field:** Status__c  
- **Update Value:** `Approved`  
- **Re-evaluation:** Workflow rules rechecked after field update.  
- **Purpose:** Automates participant approval process.  

---

## 4. Tasks
- **Task Name:** Participant Approval Task  
- **Assigned To:** Event Organizer (user).  
- **Priority:** Normal  
- **Status:** Not Started  
- **Due Date:** Configurable with offset (e.g., +2 days).  
- **Description:** “Review participant registration and confirm approval.”  

---

## 5. Approval Process
- **Object:** Participant__c  
- **Entry Criteria:** Status = `Pending`  
- **Steps:**  
  1. **Initial Submission:** Participant record submitted for approval.  
  2. **Step 1 Approver:** Automatically assigned to Organizer (or queue).  
  3. **Step 2 (Optional):** Additional approver assigned manually if required.  
- **Final Actions:**  
  - Approve → Status__c updated to `Approved`.  
  - Reject → Status__c updated to `Rejected`.  
  - Email Alerts triggered accordingly.  

---

## 6. Flow Builder Automation
- **Flow Name:** Event Attendance Flow  
- **Action:** Create record in `Event_Attendance__c` when Participant is approved.  
- **Logic:**  
  - Input: Participant record variable.  
  - Condition: Status__c = `Approved`.  
  - Action: Create related `Event_Attendance__c` record with Event ID and Participant ID.  
- **Outcome:** Tracks attendance automatically.  

---

---


---



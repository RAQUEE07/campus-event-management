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

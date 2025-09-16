🎓 Campus Event Management System
📌 Project Overview

The Campus Event Management System is a Salesforce-based application designed to simplify the organization and participation of campus events such as workshops, hackathons, cultural fests, and seminars.
It enables event organizers to create and manage events, while students can register, receive confirmations, and provide feedback — all within Salesforce.

🎯 Features

Centralized Event Management – Store and manage event details (name, date, type, venue).

Student Registration – Track student participation with automated email confirmations.

Attendance & Feedback – Capture event attendance and post-event feedback.

Dashboards & Reports – Visual insights on event popularity, student engagement, and feedback scores.

🛠 Salesforce Implementation
🔹 Custom App

Campus Events App – A Lightning App dedicated to managing events and registrations.

🔹 Custom Objects

Event

Fields: Name, Date, Type, Location, Description

Student (Contact)

Fields: Name, Email, Phone, Department, Year

Registration (Junction Object)

Fields: Student, Event, Registration Date, Attendance (Yes/No), Feedback

🔹 Automation

Flow to send an email confirmation when a student registers.

Validation Rule: Event Date must be in the future.

🔹 Reports/Dashboards

Number of students per event

Most popular event type (Technical, Cultural, Workshop)

Feedback ratings distribution

📸 Screenshots

Screenshots of setup and configurations are provided in the /Screenshots folder, including:

Salesforce Login Dashboard

App Creation

Custom Objects & Fields

Flow Automation

Validation Rules

Dashboards

🚀 How to Use

Clone this repo:

git clone https://github.com/RAQUEE07/campus-event-management.git


Import or recreate the custom objects and flows in a Salesforce Developer Org.

Use the included screenshots & documentation as guidance.

📊 Outcomes

Reduced manual effort in managing campus events.

Improved student engagement with automated communication.

Actionable insights into event performance.

👨‍💻 Author

Shaik Raqueebul Islam (RAQUEE07)

Salesforce Enthusiast | Cloud & CRM Developer

GitHub: RAQUEE07

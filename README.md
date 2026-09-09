# 📚 Learning & Study Assistant

A web-based **Learning & Study Assistant** designed to help students organize their learning activities, manage study materials, create notes, plan study schedules, practice quizzes, and track their academic progress in one place.

The application provides a simple and organized environment where students can manage their day-to-day study activities and maintain their learning progress.

---

## 📌 Project Overview

The **Learning & Study Assistant** is a full-stack web application developed to make studying more organized and productive.

Students often use different applications for notes, study schedules, learning materials, quizzes, and progress tracking. This project brings these common study activities together into a single platform.

The system allows students to:

* Manage subjects
* Upload and manage study materials
* Create and manage notes
* Create study schedules
* Set learning goals
* Practice quizzes
* Track study progress
* View performance
* Manage upcoming study tasks

---

# 🎯 Objectives

The main objectives of this project are:

1. Provide a centralized platform for student learning activities.
2. Help students organize their study materials.
3. Provide an easy-to-use note management system.
4. Help students create and maintain study schedules.
5. Allow students to practice quizzes.
6. Track learning progress.
7. Monitor quiz and study performance.
8. Help students manage their learning goals.
9. Reduce the difficulty of organizing daily study activities.
10. Provide a clean and user-friendly learning environment.

---

# ✨ Features

## 👨‍🎓 Student Module

### 🔐 User Registration & Login

Students can create and access their accounts.

Features:

* Register
* Login
* Logout
* Profile management
* Account information

---

## 🏠 Dashboard

The dashboard provides a quick overview of the student's learning activities.

It can display:

* Total subjects
* Total study materials
* Total notes
* Completed tasks
* Pending tasks
* Study goals
* Quiz scores
* Overall progress
* Recent activities

Example:

```text
---------------------------------------------
          LEARNING DASHBOARD
---------------------------------------------

Subjects              6

Study Materials       24

Notes                 35

Completed Tasks       18

Pending Tasks          5

Average Quiz Score    82%

Overall Progress      75%

---------------------------------------------
```

---

# 📚 Subject Management

Students can organize their learning based on subjects.

Example subjects:

```text
Java
Python
Database
Web Development
Operating Systems
Computer Networks
Software Engineering
```

Features:

* Add subject
* View subjects
* Edit subject
* Delete subject
* View subject details
* Track subject progress

---

# 📄 Study Material Management

Students can upload and manage their study materials.

Supported materials may include:

* PDF files
* Documents
* Text files
* Lecture notes
* Reference materials

Features:

* Upload material
* View material
* Download material
* Delete material
* Search materials
* Organize materials by subject

Example:

```text
Study Materials

Java Programming.pdf
Database Management.pdf
Operating Systems.pdf
Computer Networks.pdf
```

---

# 📝 Notes Management

Students can create and manage personal study notes.

Features:

* Create notes
* Edit notes
* Delete notes
* View notes
* Search notes
* Organize notes by subject

Example:

```text
Subject: Java

Title:
Object-Oriented Programming

Notes:
Object-oriented programming is a programming
paradigm based on objects and classes.

Topics:
- Class
- Object
- Inheritance
- Polymorphism
- Encapsulation
- Abstraction
```

---

# 📅 Study Planner

The Study Planner helps students organize their daily and weekly study activities.

Students can create:

* Study tasks
* Study sessions
* Deadlines
* Revision schedules
* Subject-wise schedules

Example:

```text
Monday

09:00 AM - Java
10:30 AM - Database

Tuesday

09:00 AM - React
11:00 AM - Operating Systems

Wednesday

09:00 AM - Computer Networks
10:30 AM - Revision
```

---

# ✅ Task Management

Students can create and track study tasks.

Features:

* Add task
* Edit task
* Delete task
* Mark task as completed
* Set due date
* Set priority
* View pending tasks

Example:

```text
Study Tasks

☑ Complete Java Collections
☑ Read DBMS Chapter 3
☐ Practice SQL Queries
☐ Revise Operating Systems
```

Task priorities:

```text
High
Medium
Low
```

---

# 🎯 Learning Goals

Students can create learning goals and track their completion.

Example:

```text
Goal:
Complete Java Programming

Start Date:
01/09/2026

Target Date:
30/09/2026

Progress:
70%
```

Other examples:

```text
Complete SQL
Learn React
Finish DBMS
Complete 10 Practice Tests
Read 5 Chapters
```

---

# 🧪 Quiz & Practice Module

Students can practice questions based on their subjects.

Features:

* Create quizzes
* Take quizzes
* Multiple-choice questions
* Submit answers
* Automatic score calculation
* View results
* Review answers
* Track previous attempts

Example:

```text
Java Quiz

1. Which keyword is used to inherit a class?

A. implements
B. extends
C. inherits
D. super

Answer:
B. extends
```

---

# 📊 Quiz Results

After completing a quiz, students can view their performance.

Example:

```text
--------------------------------
          QUIZ RESULT
--------------------------------

Subject: Java

Questions:       10
Correct:          8
Wrong:            2

Score:           80%

Performance:     Good
--------------------------------
```

Quiz history can also be maintained for future reference.

---

# 📈 Progress Tracking

The system tracks the student's learning progress.

Progress can be displayed based on:

* Subject
* Completed tasks
* Study sessions
* Quiz scores
* Learning goals
* Completed materials

Example:

```text
Java
████████████████░░░░ 80%

SQL
██████████████░░░░░░ 70%

React
███████████░░░░░░░░░ 55%

DBMS
██████████████████░░ 90%
```

---

# ⏱️ Study Session Tracking

Students can record their study sessions.

Example:

```text
Today's Study Time

Java          1 hr 20 min
SQL             45 min
React           50 min
---------------------------
Total          2 hr 55 min
```

The system can maintain a history of study sessions.

---

# 🔔 Reminders

The application can provide reminders for important study activities.

Examples:

```text
Reminder

"Java revision is scheduled for 6:00 PM."

"DBMS assignment is due tomorrow."

"Complete today's study task."
```

---

# 🔎 Search

Students can quickly search their learning content.

Search can be performed across:

* Subjects
* Notes
* Study materials
* Tasks
* Quizzes

Example:

```text
Search: inheritance
```

Possible results:

```text
Java Notes
Java Programming PDF
OOP Concepts
Java Quiz
```

---

# 📱 Responsive Design

The application is designed to work across different screen sizes.

Supported devices:

* 💻 Desktop
* 💻 Laptop
* 📱 Mobile
* 📱 Tablet

The interface should provide a consistent and user-friendly experience across devices.

---

# 🏗️ System Architecture

```text
                   ┌─────────────────┐
                   │     Student     │
                   └────────┬────────┘
                            │
                            ▼
                   ┌─────────────────┐
                   │ React Frontend  │
                   └────────┬────────┘
                            │
                         REST API
                            │
                            ▼
                   ┌─────────────────┐
                   │ Spring Boot API │
                   └────────┬────────┘
                            │
                ┌───────────┼───────────┐
                │           │           │
                ▼           ▼           ▼
         ┌──────────┐ ┌──────────┐ ┌───────────┐
         │PostgreSQL│ │  Files   │ │ Services  │
         │ Database │ │ Storage  │ │           │
         └──────────┘ └──────────┘ └───────────┘
```

---

# 💻 Technology Stack

## Frontend

* React.js
* Vite
* JavaScript
* HTML5
* CSS3
* REST API
* Fetch API / Axios

## Backend

* Java 21
* Spring Boot
* Spring Web
* Spring Data JPA
* Maven

## Database

* PostgreSQL

## File Management

* Local file storage
* Multipart file upload

## Development Tools

* IntelliJ IDEA / Eclipse
* Visual Studio Code
* Git
* GitHub
* Postman

---

# 📁 Project Structure

```text
learning-study-assistant/
│
├── backend/
│   │
│   ├── src/
│   │   └── main/
│   │       ├── java/
│   │       │   └── com/example/learning/
│   │       │
│   │       └── resources/
│   │           └── application.properties
│   │
│   ├── pom.xml
│   └── README.md
│
├── frontend/
│   │
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   ├── assets/
│   │   ├── App.jsx
│   │   └── main.jsx
│   │
│   ├── package.json
│   ├── package-lock.json
│   └── vite.config.js
│
├── uploads/
│   └── study-materials/
│
├── docker-compose.yml
│
└── README.md
```

---

# 🗄️ Database Design

The application can use PostgreSQL to store user and learning information.

Main tables:

```text
users
subjects
study_materials
notes
tasks
study_sessions
learning_goals
quizzes
questions
quiz_attempts
progress
```

### Basic Relationship

```text
User
 │
 ├── Subjects
 │      │
 │      ├── Notes
 │      ├── Study Materials
 │      ├── Tasks
 │      ├── Quizzes
 │      └── Progress
 │
 ├── Study Sessions
 │
 └── Learning Goals
```

---

# ⚙️ Prerequisites

Before running the project, install:

* JDK 21
* Node.js
* npm
* Maven
* PostgreSQL
* Git

Check installed versions:

```bash
java -version
node -v
npm -v
mvn -version
psql --version
git --version
```

---

# 🗄️ PostgreSQL Setup

Create the database:

```sql
CREATE DATABASE learning_study_db;
```

Configure the database in:

```text
backend/src/main/resources/application.properties
```

Example:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/learning_study_db
spring.datasource.username=postgres
spring.datasource.password=YOUR_PASSWORD

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

Replace:

```text
YOUR_PASSWORD
```

with your PostgreSQL password.

---

# 🚀 Backend Setup

Open a terminal and navigate to the backend:

```bash
cd backend
```

Install/build the project:

```bash
mvn clean install
```

Start the Spring Boot application:

```bash
mvn spring-boot:run
```

The backend will run at:

```text
http://localhost:8080
```

---

# ❤️ Backend Health Check

Open:

```text
http://localhost:8080/api/health
```

Expected response:

```text
Backend is running!
```

If this response appears, the backend is running successfully.

---

# 🚀 Frontend Setup

Open another terminal:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

The frontend will normally run at:

```text
http://localhost:5173
```

Open the URL in your browser.

---

# 🔗 Frontend & Backend Connection

The frontend communicates with the Spring Boot backend through REST APIs.

Example:

```javascript
fetch("http://localhost:8080/api/health")
  .then(response => response.text())
  .then(data => {
    console.log(data);
  })
  .catch(error => {
    console.error("Backend connection failed:", error);
  });
```

Expected result:

```text
Backend is running!
```

---

# 🔌 API Endpoints

## Authentication

```text
POST /api/auth/register
POST /api/auth/login
POST /api/auth/logout
```

---

## Subjects

```text
GET    /api/subjects
GET    /api/subjects/{id}
POST   /api/subjects
PUT    /api/subjects/{id}
DELETE /api/subjects/{id}
```

---

## Study Materials

```text
GET    /api/materials
GET    /api/materials/{id}
POST   /api/materials/upload
DELETE /api/materials/{id}
```

---

## Notes

```text
GET    /api/notes
GET    /api/notes/{id}
POST   /api/notes
PUT    /api/notes/{id}
DELETE /api/notes/{id}
```

---

## Tasks

```text
GET    /api/tasks
GET    /api/tasks/{id}
POST   /api/tasks
PUT    /api/tasks/{id}
DELETE /api/tasks/{id}
```

---

## Study Sessions

```text
GET    /api/study-sessions
POST   /api/study-sessions
DELETE /api/study-sessions/{id}
```

---

## Learning Goals

```text
GET    /api/goals
GET    /api/goals/{id}
POST   /api/goals
PUT    /api/goals/{id}
DELETE /api/goals/{id}
```

---

## Quizzes

```text
GET    /api/quizzes
GET    /api/quizzes/{id}
POST   /api/quizzes
POST   /api/quizzes/{id}/submit
```

---

## Progress

```text
GET    /api/progress
GET    /api/progress/{userId}
PUT    /api/progress/{id}
```

---

# 🔄 Application Workflow

```text
             Start
               │
               ▼
          User Registration
               │
               ▼
             Login
               │
               ▼
          Student Dashboard
               │
       ┌───────┼────────┐
       │       │        │
       ▼       ▼        ▼
   Subjects   Notes   Materials
       │       │        │
       └───────┼────────┘
               │
               ▼
          Study Planner
               │
               ▼
          Learning Goals
               │
               ▼
             Quiz
               │
               ▼
          Quiz Results
               │
               ▼
       Progress Tracking
               │
               ▼
              End
```

---

# 🧑‍💻 Development Workflow

The project follows a standard full-stack development workflow:

```text
Requirement Analysis
        ↓
System Design
        ↓
Database Design
        ↓
Backend Development
        ↓
REST API Development
        ↓
Frontend Development
        ↓
Frontend-Backend Integration
        ↓
Testing
        ↓
Bug Fixing
        ↓
Final Deployment
```

---

# 🧪 Testing

The project can be tested using:

### Backend Testing

* Postman
* JUnit
* Spring Boot Test

### Frontend Testing

* Browser testing
* Component testing
* Form validation
* API integration testing

### Functional Testing

Important test cases include:

```text
✓ User registration
✓ User login
✓ Subject creation
✓ Note creation
✓ Material upload
✓ Task creation
✓ Task completion
✓ Quiz submission
✓ Score calculation
✓ Progress tracking
✓ Data persistence
```

---

# 🔒 Basic Security

The application should protect user data by implementing:

* User authentication
* Password protection
* Input validation
* API validation
* File type validation
* File size validation
* Database constraints

Uploaded files should only allow supported file types.

---

# 📌 Advantages

* Simple and organized learning platform
* Centralized study management
* Easy note management
* Study schedule organization
* Quiz practice
* Progress tracking
* Subject-wise organization
* Study material management
* User-friendly interface
* Suitable for students

---

# 🚀 Future Enhancements

Possible future improvements include:

* Mobile application
* Online collaboration
* Teacher module
* Assignment management
* Attendance tracking
* Discussion forum
* Course management
* Leaderboards
* Advanced analytics
* Calendar integration
* Email notifications
* Cloud file storage
* Offline study support
* Dark mode
* Multi-language support

---

# 👥 User Roles

The current system primarily focuses on students.

Future versions can support:

```text
Student
   │
   ├── Manage Subjects
   ├── Manage Notes
   ├── Study Materials
   ├── Study Planner
   ├── Quizzes
   └── Progress

Teacher
   │
   ├── Create Courses
   ├── Upload Materials
   ├── Create Quizzes
   ├── Manage Assignments
   └── Monitor Students

Administrator
   │
   ├── Manage Users
   ├── Manage Subjects
   ├── Manage Courses
   └── System Management
```

---

# 📊 Expected Outcome

The final application provides students with a single platform to manage their complete study routine.

A student should be able to:

```text
Register
   ↓
Login
   ↓
Create Subjects
   ↓
Upload Materials
   ↓
Create Notes
   ↓
Plan Study Tasks
   ↓
Set Learning Goals
   ↓
Study
   ↓
Take Quizzes
   ↓
View Results
   ↓
Track Progress
```

---

# 📝 Conclusion

The **Learning & Study Assistant** provides a centralized solution for managing everyday academic activities.

By combining **subjects, notes, study materials, study planning, tasks, quizzes, learning goals, and progress tracking** into one application, the system helps students maintain a more structured learning routine.

The project demonstrates the development of a complete **full-stack web application** using modern frontend, backend, and database technologies.

---

# 👨‍💻 Project Information

**Project Name:** Learning & Study Assistant

**Project Type:** Full-Stack Web Application

**Frontend:** React + Vite

**Backend:** Java + Spring Boot

**Database:** PostgreSQL

**Java Version:** JDK 21

**Build Tool:** Maven

---

# 📄 License

This project is developed for **educational and academic purposes**.

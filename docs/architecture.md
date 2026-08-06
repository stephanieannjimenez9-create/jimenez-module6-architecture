
# Course Registration System - Architectural Design

## 1. System Overview

The Course Registration System is a web-based system designed to manage and simplify the course registration process of students. The system allows students to view available courses, register subjects, update registration information, and manage their enrolled courses. It also helps administrators maintain student and course records efficiently.

---

## 2. Selected Architecture Pattern


The proposed Course Registration System uses a Three-Tier Client-Server Architecture. The system is divided into three layers: Presentation Layer, Application Layer, and Data Layer.

The proposed technologies for each layer are:

- Presentation Layer: Vue.js
- Application Layer: Node.js and Express
- Data Layer: MongoDB Atlas Free

---

## 3. Architectural Components

### Presentation Layer (Vue.js)


The Presentation Layer is responsible for providing the user interface where students and administrators interact with the system.

Responsibilities:
- Display system pages and information.
- Accept user inputs.
- Send requests to the application layer.
- Display processed results to users.

### Application Layer (Node.js and Express)

The Application Layer handles the system logic and processes user requests.

Responsibilities:
- Process course registration requests.
- Validate user information.
- Manage registration operations.
- Communicate with the database.

### Data Layer (MongoDB Atlas Free)

The Data Layer stores and manages the system data.

Responsibilities:
- Store student records.
- Store course information.
- Store registration details.
- Retrieve and update database records.


The Presentation Layer provides the user interface where students and registrars interact with the system.

Responsibilities:
- Display the user interface
- Accept user input
- Send requests to the application layer
- Display system responses

### Application Layer (Node.js + Express)

The Application Layer processes user requests and manages the business logic.

Responsibilities:
- Process course registration requests
- Validate user input
- Manage application logic
- Communicate with the database

### Data Layer (MongoDB Atlas Free)

The Data Layer stores and manages all application data.

Responsibilities:
- Store student records
- Store course information
- Store registration records
- Retrieve and update data

---

## 4. System Architecture Diagram



```text
        👨‍🎓 Students / Registrar
                  |
                  v
        ┌───────────────────────┐
        │ Presentation Layer    |
        |               Vue.js  │
        └───────────────────────┘
                  |
                  v
        ┌───────────────────────┐
        │Application Layer      |
        | Node.js + Express     │
        └───────────────────────┘
                  |
                  v
        ┌───────────────────────┐
        │ Data Layer           |
        | MongoDB Atlas Free    │
        └───────────────────────┘
```
## 5. Data Flow

1. The student logs into the system.
2. The student selects a course registration function.
3. The request is sent to the Application Layer.
4. The Application Layer validates and processes the request.
5. The Data Layer stores or retrieves the required information.
6. The processed result is displayed to the user.

---

## 6. Database Design

**Database:** MongoDB Atlas Free

### Collections

- Students
- Courses
- Registrations

---
## 7. Architectural Explanation

The Course Registration System follows a Three-Tier Client-Server Architecture using Vue.js as the Presentation Layer, Node.js with Express as the Application Layer, and MongoDB Atlas Free as the Data Layer. This architecture separates the user interface, business logic, and data management, making the system easier to maintain, scalable, and suitable for future enhancements.

---

## 8. Design Justification

The Three-Tier Client-Server Architecture was selected because it separates the presentation, application, and data layers. Vue.js provides a responsive user interface, Node.js with Express efficiently processes user requests, and MongoDB Atlas Free offers flexible and scalable cloud-based data storage. This architecture improves maintainability, scalability, and overall system performance.

---

## 9. Architectural Limitations

This architectural design focuses only on the proposed structure and documentation of the Course Registration System. Source code implementation, database connectivity, authentication, deployment, and other advanced system features are outside the scope of this module.

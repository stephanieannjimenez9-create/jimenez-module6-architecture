# System Architectural Design
## 1. System Overview

The Course Registration System is a web-based application designed to simplify and manage the course registration process. It allows students to register courses, view registered courses, update registration details, drop or cancel course registrations, and search course records. The system provides a centralized platform that improves registration efficiency, minimizes manual errors, and helps academic staff manage course information effectively.

---

## 2. Selected Architecture Pattern

The proposed Course Registration System uses a Three-Tier Client-Server Architecture consisting of the Presentation Layer, Application Layer, and Data Layer. The proposed technologies are Vue.js for the presentation layer, Node.js with Express for the application layer, and MongoDB Atlas Free for the data layer.

---

## 3. Architectural Components

### Presentation Layer (Vue.js)

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
        │ DData Layer           |
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

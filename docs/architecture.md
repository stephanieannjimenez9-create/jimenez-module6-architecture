# System Architectural Design
## 1. System Overview

The Course Registration System is a web-based application designed to simplify and manage the course registration process. It allows students to register courses, view registered courses, update registration details, drop or cancel course registrations, and search course records. The system provides a centralized platform that improves registration efficiency, minimizes manual errors, and helps academic staff manage course information effectively.

---

## 2. Selected Architecture Pattern

The proposed system uses a **Three-Tier Client-Server Architecture** consisting of the Presentation Layer, Application Layer, and Data Layer. This architecture separates the user interface, business logic, and database management, making the system easier to maintain, update, and expand.

---

## 3. Architectural Components

### Presentation Layer
Provides the user interface where students and registrars interact with the system.

### Application Layer
Processes user requests, validates registration data, and manages the system's business logic.

### Data Layer
Stores and manages student records, course information, and registration data using a database.

---

## 4. System Architecture Diagram

```text
        👨‍🎓 Students / Registrar
                  |
                  v
        ┌───────────────────────┐
        │ Presentation Layer    │
        │    (Web Interface)    │
        └───────────────────────┘
                  |
                  v
        ┌───────────────────────┐
        │ Application Layer     │
        │ - Register Courses    │
        │ - View Courses        │
        │ - Update Registration │
        │ - Drop Registration   │
        │ - Search Records      │
        └───────────────────────┘
                  |
                  v
        ┌───────────────────────┐
        │ Data Layer            │
        │       MySQL DB        │
        │                       │
        │ Student Table         │
        │ Course Table          │
        │ Registration Table    │
        └───────────────────────┘
```text

5. Data Flow
The student logs into the system.
The student selects a course registration function.
The request is sent to the Application Layer.
The Application Layer validates and processes the request.
The Data Layer stores or retrieves the required information.
The processed result is displayed to the user.
6. Database Design

Database Name: course_registration_db

Tables:

Student
Course
Registration
7. Architectural Explanation

The Course Registration System follows a Three-Tier Client-Server Architecture to separate the presentation, application, and data layers. This separation improves system organization, simplifies maintenance, and allows future enhancements without affecting the entire application.

8. Design Justification

The Three-Tier Architecture was selected because it provides a clear separation of responsibilities among the user interface, application logic, and database. This makes the system more maintainable, scalable, secure, and easier to develop.

9. Architectural Limitations

This architectural design focuses only on the proposed system structure and documentation. Source code implementation, database connectivity, authentication, deployment, and other advanced features are not included in this module.

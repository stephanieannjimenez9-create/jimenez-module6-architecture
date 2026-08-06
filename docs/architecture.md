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

**Database Name:** `course_registration_db`

### Main Tables

- **Student** – Stores student information.
- **Course** – Stores course details.
- **Registration** – Stores course registration records.

---

## 7. Architectural Explanation

The Course Registration System follows a Three-Tier Client-Server Architecture, which separates the system into the Presentation Layer, Application Layer, and Data Layer. The Presentation Layer provides the user interface for students and registrars, the Application Layer processes business logic and user requests, and the Data Layer stores and manages all system data. This architecture improves system organization, simplifies maintenance, and supports future system enhancements.

---

## 8. Design Justification

The Three-Tier Client-Server Architecture was selected because it clearly separates the user interface, application logic, and database management. This design improves maintainability, scalability, security, and overall system performance, making it suitable for the proposed Course Registration System.

---

## 9. Architectural Limitations

This architectural design focuses only on the proposed structure and documentation of the Course Registration System. Source code implementation, database connectivity, authentication, deployment, and other advanced system features are outside the scope of this module.

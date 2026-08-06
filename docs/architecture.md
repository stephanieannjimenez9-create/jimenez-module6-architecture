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

---

## 4. System Architecture Diagram


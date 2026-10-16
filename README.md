# Employee–Task–Project Management System

A full-stack web application for managing employees, projects, and tasks through an integrated dashboard, with authentication, search, and filtering capabilities.

**GitHub Repository:** [SANJAY-ZZ/Dashboard-majorpr](https://github.com/SANJAY-ZZ/Dashboard-majorpr)

---

## 1. Project Overview

The Employee–Task–Project Management System is a collaborative software project designed to bring essential employee, project, and task management functions together in one web application.

The application provides a centralized interface for accessing management modules, tracking tasks, organizing projects, and viewing dashboard information. It integrates a React frontend with a Node.js and Express backend, using MongoDB for data storage.

This project was developed collaboratively by a team of seven members, with each member contributing to a designated module and the modules integrated into a single application.

## 2. Key Features

- **Authentication:** User authentication and login/logout functionality.
- **Employee Management:** Employee records and management interface.
- **Project Management:** Project organization and management.
- **Task Management:** Create, view, edit, update the status of, and delete tasks.
- **Dashboard:** Centralized dashboard with management statistics.
- **Search and Filtering:** Search and filter functionality for tasks and projects.
- **REST API:** Backend endpoints supporting dashboard, employee, project, and task operations.
- **Database Integration:** MongoDB and Mongoose integration for persistent data storage.

## 3. Technology Stack

| Layer | Technologies |
|---|---|
| Frontend | React, Vite, JavaScript |
| Styling | Tailwind CSS |
| Backend | Node.js, Express.js |
| Database | MongoDB, Mongoose |
| Authentication | JSON Web Token (JWT), bcryptjs |
| API Communication | Axios |
| Testing | Node.js test scripts, MongoMemoryServer |
| Development Tools | Git, GitHub, Visual Studio Code |

## 4. Project Modules and Team Contributions

The project was developed by seven team members. Each member is acknowledged equally as a contributor to the overall application, with individual responsibilities documented below.

| No. | Team Member | Module / Responsibility |
|---:|---|---|
| 1 | **Prethiksha** | Authentication |
| 2 | **Lakku Sindhu** | Employee Management |
| 3 | **S. Pallavika** | Project Management |
| 4 | **Angelin Sarah George** | Task Management |
| 5 | **Sanjay Kumar S** | Dashboard and Integration |
| 6 | **Debajyoti Bandyopadhyay** | Search and Filtering |
| 7 | **Harini K** | Database and REST API |

### Equal Team Acknowledgement

We acknowledge and appreciate the contributions of all seven team members to the development of the Employee–Task–Project Management System.

Each member contributed to a designated area of the project, and the combined work of the team made the integrated application possible. Module responsibilities are listed to provide transparency about individual areas of work; they do not diminish any member's contribution to the overall team project.

**Developed collaboratively by all seven team members.**

## 5. Application Architecture

The application follows a frontend–backend architecture.

```text
Employee–Task–Project Management System
                 |
        React Frontend (Vite)
                 |
        Axios API Requests
                 |
       Node.js / Express Backend
                 |
       MongoDB with Mongoose
```

- **Frontend:** Provides the user interface and management pages.
- **Backend:** Handles API requests and application logic.
- **Database:** Stores application data through MongoDB and Mongoose.
- **Integration:** Connects the frontend modules to the backend services.

## 6. Project Structure

The following is a simplified overview of the main project folders.

```text
Dashboard-majorpr/
├── backend/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── seed/
│   ├── tests/
│   ├── .env.example
│   ├── package.json
│   └── server.js
├── frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── vite.config.js
├── README.md
└── package.json
```

This tree highlights the principal directories; individual files and subdirectories may vary in the current repository.

## 7. Prerequisites

Before running the application, make sure you have:

- Node.js and npm installed.
- MongoDB installed and running locally, or access to a configured MongoDB instance.
- Git installed if you intend to clone the repository.
- A code editor such as Visual Studio Code.

## 8. Installation and Setup

### Step 1: Clone the repository

```bash
git clone https://github.com/SANJAY-ZZ/Dashboard-majorpr.git
cd Dashboard-majorpr
```

### Step 2: Install backend dependencies

```bash
cd backend
npm install
```

### Step 3: Configure the backend environment

Create a `.env` file in the backend directory using the provided `backend/.env.example` as a reference.

Configure the required MongoDB connection and other environment variables according to that example file.

**Security note:** Never commit real `.env` files, database credentials, JWT secrets, or passwords to GitHub.

### Step 4: Start the backend

From the project root, run:

```bash
npm run start:backend
```

The backend is configured to use port `5000` in the current development setup.

### Step 5: Install frontend dependencies

Open a second terminal in the project root and run:

```bash
cd frontend
npm install
```

### Step 6: Start the frontend

From the project root, run:

```bash
npm run start:frontend
```

Vite typically serves the frontend at:

```text
http://localhost:5173
```

Keep the backend and frontend terminals running while using the application.

### Optional: Seed the database

If you need to initialize or repopulate the database, review the seed script first and then run the following command from the project root:

```bash
npm run seed
```

Use this command only when appropriate for your database setup, because seeding may insert or modify records.

## 9. Backend API

The backend exposes endpoints for application health, dashboard statistics, and management resources.

| Endpoint | Purpose |
|---|---|
| `GET /api/health` | Check backend health |
| `GET /api/dashboard/stats` | Retrieve dashboard statistics |
| `/employees` | Employee resource operations |
| `/projects` | Project resource operations |
| `/tasks` | Task resource operations |

The employee, project, and task resource paths above represent the API paths used by the application. The exact supported HTTP methods and request formats depend on the implemented backend routes.

## 10. Testing and Verification

The following checks have been performed during development:

- Authentication and login/logout functionality.
- Dashboard, employee, project, and task management pages.
- Task creation, editing, status updates, and deletion.
- Search and filtering functionality for tasks and projects.
- Persistence of task data and task status updates in the configured MongoDB database.
- Frontend production build using Vite.

The frontend production build completed successfully with Vite 5.4.21, transforming 1,644 modules.

The backend automated test suite was also reported to pass 124 tests across four test suites. Those automated tests use MongoMemoryServer for an in-memory test database; this result should be distinguished from the separate manual checks against the configured application database.

### Run the backend tests

From the project root:

```bash
npm run test:backend
```

### Build the frontend for production

From the project root:

```bash
npm run build:frontend
```

The frontend build output is generated in `frontend/dist/`.

## 11. Screenshots

Screenshots can be added to a `screenshots/` directory in the repository to demonstrate the application's interface.

Recommended screenshots:

- Login page
- Dashboard
- Employee Management
- Project Management
- Task Management
- Search and Filtering

After adding the actual screenshot files, include them here using Markdown image links. For example:

```markdown
![Dashboard](screenshots/dashboard.png)
```

Use the actual filenames of the screenshots saved in the repository.

## 12. Future Improvements

Potential future improvements include:

- Adding more automated integration tests.
- Improving validation and error handling across modules.
- Expanding reporting and analytics capabilities.
- Enhancing accessibility and responsive layouts.
- Adding deployment documentation and production environment configuration.

These are possible future enhancements, not claims about currently implemented features.

## 13. Repository

Explore the source code, review the project structure, and follow the development work here:

**[Open the GitHub Repository](https://github.com/SANJAY-ZZ/Dashboard-majorpr)**

## 14. Acknowledgements

We sincerely acknowledge all seven team members for their collaborative work on the Employee–Task–Project Management System.

The project represents a combined effort across authentication, employee management, project management, task management, dashboard integration, search and filtering, and database/API development.

**Project:** Employee–Task–Project Management System
**Team size:** 7 members
**Repository:** [SANJAY-ZZ/Dashboard-majorpr](https://github.com/SANJAY-ZZ/Dashboard-majorpr)

*Built collaboratively as a team software development project.*

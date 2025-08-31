# JWT Web Application

A small web application built with **Django** and **React**, featuring **JWT authentication**, **PostgreSQL database**, and **Redux** for global state management. The app includes both **user** and **admin** functionality and is fully **Dockerized** for easy setup.

---

## Features

### User Side
- **Login / Register** with JWT authentication
- **Home Page** with navigation to the **Profile Page**
- **User Profile Page** with the ability to **upload profile image**

### Admin Side
- **Admin Login**
- **View and search** user data
- **Create, edit, and delete** user data

---

## Technologies Used
- **Backend:** Django, Django REST Framework
- **Frontend:** React, Redux
- **Database:** PostgreSQL
- **Authentication:** JWT (JSON Web Tokens)
- **Containerization:** Docker, Docker Compose

---

## Installation

1. **Clone the repository**
```bash
git clone https://github.com/rahilaaaa/admin_management

```

2. **Setup Instructions**

### 1. Set up environment variables
- **Backend:** `backend/sample_jwt/.env`
- **Frontend:** `frontend/auth_demo/.env`

### 2. Build and run Docker containers
```bash
docker-compose up --build
```
3. Apply backend migration
 ```bash
   docker-compose exec backend python manage.py migrate
```
4. **Access the app**
Frontend: http://localhost:5173
Backend API: http://localhost:8000

###Usage

Register as a new user or login as an admin
Navigate between Home and Profile pages
Admin can manage user data via search and CRUD operations

# Project Folder Structure


project-root/
├── backend/
│ └── sample_jwt/ # Django backend
├── frontend/
│ └── auth_demo/ # React frontend
├── docker-compose.yaml
├── README.md
└── .gitignore

Notes

Profile images and media files are stored in backend/sample_jwt/media/
Docker ensures all services (backend, frontend, and PostgreSQL) run in isolated containers



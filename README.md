# JWT Web Application

A small web application built with **Django** and **React**, featuring **JWT authentication**, **PostgreSQL database**, and **Redux** for global state management. The app includes both **user** and **admin** functionality and is fully **Dockerized** for easy setup.

---

## 🚀 Features

### 👤 User Side
- **Login / Register** with JWT authentication  
- **Home Page** with navigation to the **Profile Page**  
- **Profile Page** with the ability to **upload profile image**  

### 🛠️ Admin Side
- **Admin Login**  
- **View and search** user data  
- **Create, edit, and delete** user data  

---

## 🧑‍💻 Technologies Used
- **Backend:** Django, Django REST Framework  
- **Frontend:** React, Redux  
- **Database:** PostgreSQL  
- **Authentication:** JWT (JSON Web Tokens)  
- **Containerization:** Docker, Docker Compose  

---

## ⚙️ Installation (Quick Steps)

### Step-by-Step Setup Guide

| Step | Command / Instruction | Description |
|------|------------------------|-------------|
| **1** | ```bash git clone https://github.com/rahilaaaa/admin_management ``` | Clone the repository |
| **2** | ```bash pip install -r requirements.txt ``` | Install Python dependencies |
| **3** | Create `.env` file inside `backend/sample_jwt/` | Add your environment variables (DB, secret key, etc.) |
| **4** | ```bash docker compose up db ``` | Start PostgreSQL database container |
| **5** | ```bash docker compose up backend ``` | Start Django backend container |
| **6** | ```bash docker compose exec backend python manage.py migrate ``` | Apply database migrations |
| **7** | ```bash docker compose exec backend python manage.py createsuperuser ``` | Create Django admin user |
| **8** | ```bash docker compose up frontend ``` | Start React frontend container |
| **9** | Visit: [http://localhost:5173](http://localhost:5173) | Open frontend in browser |
| **10** | Visit: [http://localhost:8000](http://localhost:8000) | Access backend API |

---

## 🌐 Access the App
- **Frontend:** [http://localhost:5173](http://localhost:5173)  
- **Backend API:** [http://localhost:8000](http://localhost:8000)  

---

## 📌 Usage
- Register as a new user or login as an admin  
- Navigate between **Home** and **Profile** pages  
- Admin can manage user data via **search** and **CRUD operations**  

---

## 📝 Notes
- Profile images and media files are stored in:
  backend/sample_jwt/media/


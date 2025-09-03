

# 📝 Task Manager API (Django REST Framework)

## 🚀 Overview
Ye ek simple Task Manager API hai jo Django REST Framework (DRF) se banayi gayi hai.  
Isme user authentication (JWT) ke saath tasks create, read, update aur delete karne ki facility hai.  

---

## ⚙️ Features
- User Registration & JWT Authentication
- Create, Read, Update, Delete (CRUD) tasks
- Task ownership (har user ke apne tasks)
- Search tasks by title
- API browsable interface (DRF)

---

## 📦 Installation
bash
git clone <repo-url>
cd backend/database_integration
python -m venv venv
venv\Scripts\activate   # (Windows)
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
🔑 Authentication
JWT token generate karne ke liye:

bash
Copy code
POST /api/token/
{
  "username": "your_username",
  "password": "your_password"
}
Refresh token:

swift
Copy code
POST /api/token/refresh/
📌 API Endpoints
Auth
POST /register/ → Register user

POST /api/token/ → Get JWT token

POST /api/token/refresh/ → Refresh token

Tasks
GET /tasks/ → List all tasks (Auth required)

POST /tasks/ → Create new task

PUT /tasks/<id>/ → Update task

DELETE /tasks/<id>/ → Delete task

GET /tasks/?search=<keyword> → Search tasks by title

🛠️ Tech Stack
Python 3.12

Django 5.x

Django REST Framework

SimpleJWT

Author
Priyanshu

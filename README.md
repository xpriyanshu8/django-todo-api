

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



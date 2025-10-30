<h1 align="center">📘 Django REST API – Tutorials CRUD Application</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.11-blue?logo=python" />
  <img src="https://img.shields.io/badge/Django-REST%20Framework-red?logo=django" />
  <img src="https://img.shields.io/badge/MySQL-Database-orange?logo=mysql" />
  <img src="https://img.shields.io/badge/CRUD-Create--Read--Update--Delete-success" />
</p>

---

## 📋 Overview

This project implements a **Django REST API** for managing tutorials.  
It demonstrates the use of **Function-Based Views (FBVs)** and **Class-Based Views (CBVs)** in Django REST Framework (DRF).  

Each tutorial includes a **title**, **description**, and **published** status.

The API supports:
- ✅ Listing all tutorials
- ✅ Filtering by title
- ✅ Creating new tutorials
- ✅ Updating and deleting tutorials
- ✅ Retrieving only published tutorials

---

## 🧩 Tech Stack

| Layer | Technology |
|-------|-------------|
| **Backend** | Django, Django REST Framework |
| **Database** | MySQL |
| **Language** | Python |
| **Tools** | Postman / cURL |

---

## 🚀 API Endpoints

| HTTP Method | Endpoint | Description |
|--------------|-----------|--------------|
| `GET` | `/django_rest_api/tutorials/` | List all tutorials |
| `POST` | `/django_rest_api/tutorials/` | Create new tutorial(s) |
| `DELETE` | `/django_rest_api/tutorials/` | Delete all tutorials |
| `GET` | `/django_rest_api/tutorials/<id>/` | Retrieve tutorial by ID |
| `PUT` | `/django_rest_api/tutorials/<id>/` | Update tutorial |
| `DELETE` | `/django_rest_api/tutorials/<id>/` | Delete tutorial |
| `GET` | `/django_rest_api/tutorials/published/` | List all published tutorials |

---

## ⚙️ Setup Instructions

1️⃣ Clone this repository  
```bash
git clone https://github.com/khushi25py/DjangoRestApi-Tutorials.git
cd DjangoRestApi-Tutorials
2️⃣ Create virtual environment
python -m venv venv
venv\Scripts\activate
3️⃣ Install dependencies
pip install -r requirements.txt
4️⃣ Set up database in MySQL and update credentials in settings.py
Example:
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'testdb',
        'USER': 'root',
        'PASSWORD': '',
        'HOST': 'localhost',
        'PORT': '3306'
    }
}

5️⃣ Apply migrations and run server
python manage.py migrate
python manage.py runserver

Access API: 👉 http://127.0.0.1:8000/django_rest_api/tutorials/

🧠 Validation Rules
Title must be at least 3 characters
Description must be at least 20 characters
Title and description cannot be the same

💡 Future Enhancements
✅ Add Swagger API Docs
✅ Add JWT Authentication
✅ Pagination & Filters
✅ Swagger + ReDoc Integration

👩‍💻 Author
Khushi Gupta


<p align="center">
  Built with ❤️ using <strong>Django REST Framework</strong>
</p>



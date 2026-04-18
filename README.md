# 🏥 Hospital Management System

A production-ready **Hospital Management System** built using **Django (Python)** and **Django REST Framework**, designed to manage core hospital operations such as patients, doctors, appointments, and billing.

This project focuses on **backend architecture, API development, authentication, and scalable system design**, simulating real-world healthcare backend systems.

---

## 🚀 Features

### 👨‍⚕️ Doctor Management
- Add, update, and manage doctor profiles
- View assigned appointments
- Handle patient interactions

### 🧑‍🤝‍🧑 Patient Management
- Register and manage patient records
- Store medical history and details
- Track appointment history

### 📅 Appointment Scheduling
- Book and manage appointments
- Conflict detection and time-slot management
- Track upcoming and completed appointments

### 💳 Billing System
- Generate and manage billing records
- Maintain structured transaction history

### 🔐 Authentication & Authorization
- Secure login & registration system
- JWT-based authentication
- Role-based access control (Admin/Doctor/Patient)
- Protected API endpoints

---

## 🛠️ Tech Stack

- **Backend:** Django, Django REST Framework
- **Database:** SQLite (dev) / PostgreSQL (production-ready)
- **Authentication:** JWT (SimpleJWT)
- **Caching:** Redis
- **Server:** Gunicorn
- **Static Files:** Whitenoise
- **Environment Config:** python-dotenv
- **Version Control:** Git & GitHub

---

## 📦 Requirements

```
asgiref==3.11.1
async-timeout==5.0.1
Django==5.2.11
django-redis==6.0.0
djangorestframework==3.16.1
djangorestframework-simplejwt==5.5.1
gunicorn==25.1.0
packaging==26.0
psycopg2-binary==2.9.11
PyJWT==2.11.0
python-dotenv==1.2.1
redis==7.2.0
sqlparse==0.5.5
tzdata==2025.3
whitenoise==6.11.0
dj-database-url==2.1.0
```

---

## 📂 Project Structure

```
hospital-management-system/
│
├── project/              # Django project settings
├── users/                # Authentication & user roles
├── patients/             # Patient management module
├── doctors/              # Doctor management module
├── appointments/         # Appointment scheduling logic
├── billing/              # Billing & transactions
├── templates/            # HTML templates
├── static/               # Static files
├── db.sqlite3
└── manage.py
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone Repository
```bash
[git clone https://github.com/your-username/hospital-management-system.git]
```

### 2️⃣ Create Virtual Environment
```bash
python -m venv venv
```

Activate:
- Windows:
```bash
venv\Scripts\activate
```
- Mac/Linux:
```bash
source venv/bin/activate
```

### 3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 4️⃣ Setup Environment Variables
Create a `.env` file in root directory:

```
DEBUG=True
SECRET_KEY=your_secret_key
DATABASE_URL=your_database_url
```

---

### 5️⃣ Apply Migrations
```bash
python manage.py makemigrations
python manage.py migrate
```

### 6️⃣ Run Development Server
```bash
python manage.py runserver
```

Open:
http://127.0.0.1:8000/

---

## 🌐 Run in Production (Optional)

```bash
gunicorn project.wsgi:application
```

---

## 🔗 API Overview (Sample)

- `POST /api/auth/login/` → User login (JWT)
- `POST /api/auth/register/` → User registration
- `GET /api/patients/` → Fetch all patients
- `POST /api/appointments/` → Book appointment
- `GET /api/doctors/` → List doctors
- `GET /api/billing/` → View billing records

---

## 🧠 Key Backend Concepts Implemented

- REST API design and development
- JWT-based authentication and authorization
- Relational database design (Patients, Doctors, Appointments, Billing)
- Caching using Redis for performance optimization
- Data validation and error handling
- Modular and scalable backend architecture
- Production deployment setup using Gunicorn

---

## 📊 Future Enhancements

- Full frontend integration (React / Flutter)
- Payment gateway integration
- Email/SMS notifications
- Admin analytics dashboard
- Docker containerization
- Deployment on AWS / Render

---

## 📜 License

This project is created for educational and learning purposes.

---

## 👨‍💻 Author

Lakshay Bishnoi  
B.Tech CSE Student

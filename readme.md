# 🌍 Garbage Map – Smart Waste Reporting & Management System

## 📌 Project Description

Garbage Map is a full-stack web application built using **Python Django** to tackle urban waste management problems by enabling citizens to report garbage locations in real time. The platform allows users to upload images, tag locations on a map, and notify authorities for quick action.

This system bridges the gap between citizens and municipal authorities by providing a transparent and efficient workflow for reporting, tracking, and resolving waste-related issues.

The project can be extended using AI to automatically classify garbage types, detect severity, and prioritize clean-up operations.

---

## 🚀 Key Features

### 👤 User Features

* Register and login securely
* Report garbage by:

  * Uploading images
  * Selecting location on map
  * Adding description
* View reported garbage spots on map
* Track status (Pending / In Progress / Resolved)

### 🛠️ Admin Features

* Admin dashboard using Django Admin Panel
* View and manage all reports
* Update complaint status
* Monitor high-priority areas

### 🤖 AI Features (Optional/Advanced)

* Image classification (garbage vs non-garbage)
* Severity detection (low, medium, high)
* Duplicate detection

---

## 🧠 Problem Statement

Urban areas face significant challenges in managing waste due to lack of proper reporting systems and delayed responses. Citizens often don’t have an easy way to notify authorities about garbage accumulation.

Garbage Map solves this by:

* Providing a centralized reporting system
* Enabling faster response from authorities
* Improving city cleanliness through data-driven decisions

---

## 💡 Solution Overview

The application uses a Django-based architecture:

* **Backend Framework:** Django (Python)
* **Frontend:** HTML, CSS, JavaScript (or Django Templates)
* **Database:** SQLite (development) / PostgreSQL (production)
* **Media Storage:** Django Media Files / Cloudinary
* **Maps Integration:** Google Maps API / Leaflet.js

Users submit reports → Stored in database → Displayed on map → Admin updates status → Users get updates

---

## 🗂️ Project Structure

```
garbage_map/
│── manage.py
│── db.sqlite3
│
├── garbage_map/        # Main project folder
│   ├── settings.py
│   ├── urls.py
│
├── reports/            # App for garbage reports
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│   ├── templates/
│   ├── static/
```

---

## 📊 Database Models (Basic)

### User (Django Default/User Extension)

* username
* email
* password
* role (optional)

### Report Model

* image
* location (latitude, longitude)
* description
* status
* created_by
* created_at

---

## 🛠️ Tech Stack

* Python
* Django
* HTML, CSS, JavaScript
* SQLite / PostgreSQL
* Google Maps API / Leaflet

---

## 🔄 Workflow

1. User logs in
2. Reports garbage with image + location
3. Data stored in database
4. Admin reviews and updates status
5. Issue gets resolved and updated on map

---

## 📈 Future Enhancements

* AI-based garbage detection using ML models
* Heatmap for garbage-prone areas
* Notification system (Email/SMS)
* Mobile app version
* Integration with municipal systems

---

## 💰 Revenue Model (Important for Viva)

* Government partnerships
* SaaS model for municipalities
* Data insights for urban planning
* Sponsored cleanliness campaigns

---

## 🎯 Why This Project Stands Out

* Solves real-world problem
* Scalable for smart cities
* Combines Web + Maps + AI
* Strong social impact

---

## 🧪 How to Run Locally

### 1. Clone repository

```
git clone <repo-link>
cd garbage_map
```

### 2. Create virtual environment

```
python -m venv venv
source venv/bin/activate   # On Windows: venv\\Scripts\\activate
```

### 3. Install dependencies

```
pip install -r requirements.txt
```

### 4. Run migrations

```
python manage.py migrate
```

### 5. Run server

```
python manage.py runserver
```


## 👩‍💻 Author

Shariya Ansari

---

## 📜 License

This project is developed for learning and open source contribution.

# Daily Task Tracker — Django Web Application

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-4.x-092E20?logo=django&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-5-7952B3?logo=bootstrap&logoColor=white)
![SQLite](https://img.shields.io/badge/Database-SQLite-003B57?logo=sqlite&logoColor=white)

## Overview

Full-stack web application for **personal task management and productivity tracking**, built with Django.
Users can log daily tasks, monitor completion over time, and view interactive charts of their productivity trends — all through a responsive, mobile-friendly interface.

Demonstrates end-to-end Django development: authentication, ORM, CRUD views, URL routing, custom template tags, and Chart.js integration.

---

## Features

| Feature | Implementation |
|---------|---------------|
| User authentication | Django `auth` — register, login, logout |
| Task CRUD | Create, read, update, delete via Django ORM |
| Completion tracking | Date-range filtering with completion percentage |
| Interactive charts | `generate_plot()` — task completion trend over time |
| Completion KPI | `calculate_completion_percentage()` — daily/weekly stats |
| Admin dashboard | Django admin panel for user and task management |
| Responsive UI | Bootstrap 5 — mobile and desktop optimised |

---

## Setup

```bash
git clone https://github.com/sylver86/19-daily-task-tracker-django.git
cd 19-daily-task-tracker-django

# Create virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install dependencies
pip install django

# Apply migrations
python manage.py migrate

# Create admin user
python manage.py createsuperuser

# Run development server
python manage.py runserver
```

Open `http://127.0.0.1:8000` in your browser.
Admin panel available at `http://127.0.0.1:8000/admin`.

---

## Project Structure

```
19-daily-task-tracker-django/
├── manage.py
├── mydailytracker/        # Django project settings
├── tracker/               # Main app
│   ├── models.py          # Task model
│   ├── views.py           # CRUD views + chart generation
│   ├── urls.py            # URL routing
│   └── templates/         # Bootstrap HTML templates
└── urls.py                # Root URL configuration
```

---

## Technologies

`Python 3.10+` · `Django 4.x` · `SQLite` · `Bootstrap 5` · `Chart.js` · `Django ORM`

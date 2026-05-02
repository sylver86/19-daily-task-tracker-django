# DailyTrack — Web Application Full-Stack per Gestione Task (Django)

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-4.x-092E20?logo=django&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-5-7952B3?logo=bootstrap&logoColor=white)
![SQLite](https://img.shields.io/badge/Database-SQLite-003B57?logo=sqlite&logoColor=white)

## Panoramica

Web application full-stack Django per la gestione personale di task e il monitoraggio della produttività. Gli utenti registrano task giornalieri, tracciano il completamento nel tempo e visualizzano grafici interattivi dell'andamento — tutto tramite un'interfaccia responsive mobile-friendly.

Dimostra sviluppo web Django end-to-end: autenticazione utente, ORM per CRUD, routing URL, template tag custom e integrazione Chart.js — stack applicativo scalabile verso REST API, microservizi e soluzioni enterprise.

## Valore Enterprise

| Settore / Azienda | Rilevanza |
|-------------------|-----------|
| Engineering Informatica | Web app Django su stack Python enterprise |
| IT Consulting (NTT Data, Accenture) | Full-stack Python per portali interni enterprise |
| Qualsiasi settore | Pattern CRUD + autenticazione applicabile a tool interni |
| Data Reply | Django come base per data product con UI integrata |

## Funzionalità

| Feature | Implementazione |
|---------|----------------|
| Autenticazione utente | Django `auth` — registrazione, login, logout |
| CRUD task | Create, read, update, delete via Django ORM |
| Tracking completamento | Filtro per date con percentuale di completamento |
| Grafici interattivi | `generate_plot()` — trend completamento nel tempo |
| KPI completamento | `calculate_completion_percentage()` — stats giornaliere/settimanali |
| Admin dashboard | Pannello Django admin per gestione utenti e task |
| UI responsive | Bootstrap 5 — ottimizzato per mobile e desktop |

## Setup

```bash
git clone https://github.com/sylver86/19-daily-task-tracker-django.git
cd 19-daily-task-tracker-django

python -m venv venv && source venv/bin/activate
pip install django

python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

Apri `http://127.0.0.1:8000` nel browser.
Admin panel: `http://127.0.0.1:8000/admin`.

## Struttura Progetto

```
19-daily-task-tracker-django/
├── manage.py
├── mydailytracker/        # Settings Django
├── tracker/               # App principale
│   ├── models.py          # Modello Task
│   ├── views.py           # CRUD views + generazione grafici
│   ├── urls.py            # Routing URL
│   └── templates/         # Template HTML Bootstrap
└── urls.py                # Configurazione URL root
```

## Stack Tecnologico

`Python 3.10+` · `Django 4.x` · `SQLite` · `Bootstrap 5` · `Chart.js` · `Django ORM`

---

---

# DailyTrack — Full-Stack Task Management Web Application (Django) 🇬🇧

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-4.x-092E20?logo=django&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-5-7952B3?logo=bootstrap&logoColor=white)

## Overview

Full-stack Django web application for personal task management and productivity tracking. Users log daily tasks, monitor completion over time, and view interactive charts of productivity trends — through a responsive, mobile-friendly interface.

Demonstrates end-to-end Django development: user authentication, ORM CRUD, URL routing, custom template tags, and Chart.js integration — a scalable foundation towards REST APIs, microservices, and enterprise solutions.

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

## Setup

```bash
git clone https://github.com/sylver86/19-daily-task-tracker-django.git
cd 19-daily-task-tracker-django

python -m venv venv && source venv/bin/activate
pip install django

python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

Open `http://127.0.0.1:8000`. Admin at `http://127.0.0.1:8000/admin`.

## Project Structure

```
19-daily-task-tracker-django/
├── manage.py
├── mydailytracker/        # Django project settings
├── tracker/               # Main app (models · views · urls · templates)
└── urls.py                # Root URL configuration
```

## Technologies

`Python 3.10+` · `Django 4.x` · `SQLite` · `Bootstrap 5` · `Chart.js` · `Django ORM`

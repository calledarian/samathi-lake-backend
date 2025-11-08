# Samathi Lake Backend

This is the backend API for the **Samathi Lake admin panel**, built with **Django + Django REST Framework + JWT authentication**.  
It provides endpoints for authentication, and will later handle admin features like managing tours, bookings, and user data.

## Features

- JWT authentication (`access` & `refresh` tokens)  
- User management (Django admin & custom API endpoints)  
- SQLite database for development (can switch to PostgreSQL for production)  
- CORS enabled for Next.js frontend (`http://localhost:3000`)

## Requirements

- Python 3.12+
- pip
- Virtualenv

## Setup / Installation

```bash
git clone <your-repo-url>
cd sl-backend

Create a virtual environment:

python -m venv .venv
source .venv/bin/activate  # Linux/macOS

pip install -r requirements.txt

python manage.py migrate

python manage.py createsuperuser

python manage.py runserver

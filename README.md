# API Authentication

## Overview

The API Authentication project demonstrates how to implement authentication and authorization in a Django REST Framework (DRF) application. This project includes features for user registration, login, and permissions management to secure API endpoints.

## Features

- **User Registration**: Allows users to create new accounts.
- **User Login**: Authenticates users and generates tokens.
- **Token Authentication**: Secures API endpoints using token-based authentication.
- **Custom Permissions**: Defines and enforces custom permissions for different user roles.

## Requirements

- Python 3.x
- Django 3.x or later
- Django REST Framework (DRF) 3.x or later

## Installation

1. **Clone the Repository**

    ```bash
    git clone https://github.com/karimtz999/API_Authentication.git
    cd API_Authentication
    ```

2. **Create a Virtual Environment**

    ```bash
    python -m venv env
    source env/bin/activate  # On Windows use `env\Scripts\activate`
    ```

3. **Install Dependencies**

    ```bash
    pip install -r requirements.txt
    ```

4. **Apply Migrations**

    ```bash
    python manage.py migrate
    ```

5. **Create a Superuser**

    ```bash
    python manage.py createsuperuser
    ```

6. **Run the Development Server**

    ```bash
    python manage.py runserver
    ```

## Usage

### Endpoints

- **Register User**: `POST /api/register/`
- **Login User**: `POST /api/login/`
- **Logout User**: `POST /api/logout/`
- **Profile**: `GET /api/profile/`

### Example Requests

**Register User**

```bash
curl -X POST http://localhost:8000/api/register/ -d '{"username": "user1", "password": "pass123"}' -H "Content-Type: application/json"

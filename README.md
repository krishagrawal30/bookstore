# 📚 Django Bookstore Management System

## 1. Project Overview

This is a Django-based Bookstore Management System that allows users to:
- View a list of books (with title, author, and price)
- Add books to a session-based cart
- View and manage cart items
- Login and logout securely

Built using only Class-Based Views and custom templates, without Django Forms or the default admin panel.

---

## 2. Setup & Run Instructions

### Clone the Repository

```bash
git clone https://github.com/yourusername/bookstore-django.git
cd bookstore-django

```
## 3. Set Up Virtual Environment
python3 -m venv env
source env/bin/activate
pip install -r requirements.txt
- Run Migrations
python manage.py makemigrations
python manage.py migrate
- Create Superuser (Optional)
python manage.py createsuperuser
- Start the Server
python manage.py runserver
Visit http://127.0.0.1:8000/store/login/ to start.

## 3. Tech Stack Used
Backend: Django 4.x (Python 3.12)

Frontend: HTML (custom templates)

Session Management: Django sessions

DevOps: Docker, Jenkins

## 🐳 Docker
This project includes a Dockerfile and docker-compose.yml for containerized deployment.

Steps to run with Docker:
Build the image
docker-compose build
 Run the container
docker-compose up

## Jenkins
To automate deployment and testing, a Jenkinsfile is included in the root of the project.

Basic pipeline stages:

Checkout: Pulls the latest code

Install Dependencies: Installs packages from requirements.txt

Run Migrations: Applies Django database migrations

Run Server: Starts the Django app

Steps to run Jenkins pipeline:

Install Jenkins and required plugins (Pipeline, Docker, etc.)

Create a new pipeline job in Jenkins.

Point it to this repository.

Run the pipeline.

This setup ensures continuous integration and consistent deployment using Jenkins and Docker.

# Insurance Management (Django)

A Django-based Insurance Management System with customer and admin flows.

## Quick Start

1. Create and activate a virtual environment (already configured in `.venv`).
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run migrations:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```
4. Create a superuser:
   ```bash
   python manage.py createsuperuser
   ```
5. Start the development server:
   ```bash
   python manage.py runserver
   ```

## Project Structure

- `insurancemanagement/` – Django project settings and URLs
- `insurance/` – Admin-facing app (policies, categories, approvals)
- `customer/` – Customer-facing app (signup, dashboard, apply policy)
- `templates/` – HTML templates for both apps
- `static/` – Static assets

## Deployment

- Configure environment variables and a production database.
- Collect static files:
  ```bash
  python manage.py collectstatic
  ```
- Use a WSGI/ASGI server (e.g., Gunicorn/Uvicorn) behind Nginx.

## GitHub

To publish this project:

```powershell
# From the nested project directory
cd C:\Users\shivk\Downloads\insurance_management\insurance_management

# Initialize git and commit
git init
git add .
git commit -m "Initial commit: Insurance Management"

# Create a GitHub repo (replace USER and REPO)
git remote add origin https://github.com/USER/REPO.git

# Push the main branch
git branch -M main
git push -u origin main
```

> Tip: Add secrets/config in `.env` and do not commit it.

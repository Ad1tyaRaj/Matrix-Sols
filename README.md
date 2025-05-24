# Matrix Sols – Developer Task

## 🚀 Setup Instructions

1. Clone the repo or extract the ZIP.
2. Create a virtual environment:
python -m venv env
source env/bin/activate # or env\Scripts\activate on Windows


3. Install requirements:
pip install -r requirements.txt

4. Run migrations:
python manage.py makemigrations
python manage.py migrate

5. Create a user:
python manage.py createsuperuser

6. Run the server:
python manage.py runserver


---

As Example
In  UIUX  all things include

## 🔑 Test Credentials

- **Username**: `user`
- **Password**: `xxxxx`
- Obtain JWT token:
- `POST /login/` with `{ "username": "testuser", "password": "xxxxxx" }`

---

## 📘 API Summary

### Public:
- `GET /notes/` – List notes
- `POST /notes/` – Create note

### Auth Required:
- `GET /notes/<id>/` – View own note
- `GET /notes/?search=...` – Search notes
- JWT Token: `POST /api/token/`
- Refresh Token: `POST /api/token/refresh/`

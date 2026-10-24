# Django Mini Project: Student Management System

A beginner-friendly Django CRUD project to add, view, edit, and delete student records.

## Features
- Dashboard with student count
- Add student
- View student list and search by name/course
- Edit student
- Delete student with confirmation
- SQLite database
- Responsive styling

## Run on Windows (PowerShell)

1. Extract the ZIP.
2. Open the extracted `django_mini_project` folder in VS Code.
3. Open Terminal in that folder. Confirm `manage.py` is visible with `dir`.
4. (Optional but recommended) Create and activate a virtual environment:

   ```powershell
   python -m venv .venv
   .\.venv\Scripts\Activate.ps1
   ```

   If PowerShell blocks activation, use `.\.venv\Scripts\python.exe` in the commands below, or run `Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass`.

5. Install Django:

   ```powershell
   python -m pip install -r requirements.txt
   ```

6. Create the database tables:

   ```powershell
   python manage.py migrate
   ```

7. Start the development server:

   ```powershell
   python manage.py runserver
   ```

8. Open http://127.0.0.1:8000/ in your browser.

## Optional admin panel

Create an admin user:

```powershell
python manage.py createsuperuser
```

Then visit http://127.0.0.1:8000/admin/

## Important
This is a learning project. Before production deployment, set a secure `SECRET_KEY`, configure `DEBUG=False`, configure `ALLOWED_HOSTS`, and use a production database/server.

# Login System Project

This project is a simple login system built using Django for the backend and HTML, CSS, and JavaScript for the frontend. It allows users to register, log in, and manage their sessions.

## Project Structure

```
login-system
├── backend
│   ├── manage.py
│   ├── db.sqlite3
│   ├── requirements.txt
│   ├── login_system
│   │   ├── __init__.py
│   │   ├── asgi.py
│   │   ├── settings.py
│   │   ├── urls.py
│   │   └── wsgi.py
│   └── users
│       ├── __init__.py
│       ├── admin.py
│       ├── apps.py
│       ├── migrations
│       │   └── __init__.py
│       ├── models.py
│       ├── tests.py
│       └── views.py
├── frontend
│   ├── index.html
│   ├── css
│   │   └── styles.css
│   └── js
│       └── scripts.js
└── README.md
```

## Technologies Used

- **Backend**: Django, Python
- **Database**: MySQL (or SQLite for development)
- **Frontend**: HTML, CSS, JavaScript

## Setup Instructions

1. **Clone the repository**:
   ```
   git clone <repository-url>
   cd login-system
   ```

2. **Set up the backend**:
   - Navigate to the `backend` directory.
   - Create a virtual environment:
     ```
     python -m venv venv
     source venv/bin/activate  # On Windows use `venv\Scripts\activate`
     ```
   - Install the required packages:
     ```
     pip install -r requirements.txt
     ```

3. **Configure the database**:
   - Update the `settings.py` file in the `login_system` directory to configure your MySQL database settings.

4. **Run migrations**:
   ```
   python manage.py migrate
   ```

5. **Create a superuser** (optional):
   ```
   python manage.py createsuperuser
   ```

6. **Run the server**:
   ```
   python manage.py runserver
   ```

7. **Access the frontend**:
   - Open `frontend/index.html` in your web browser to view the login page.

## Usage

- Users can register and log in using the provided forms.
- Admins can manage users through the Django admin interface.

## Contributing

Feel free to fork the repository and submit pull requests for any improvements or features you would like to add.
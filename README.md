# Thermos

This repository contains a Flask web application for user registration, login, and basic authentication features. The application utilizes SQLite for data storage and Flask-Session for session management. Below is an overview of the code structure and its functionalities.

## Code Overview

### File Structure

- `app.py`: Contains the main Flask application code with routes and configuration.
- `templates/`: Directory containing HTML templates for rendering pages.
- `users.db`: SQLite database file to store user data.
- `apology.html`: HTML template for rendering error messages.

### Key Dependencies

- **Flask**: A micro web framework for Python.
- **Flask-Session**: An extension for managing user sessions in Flask.
- **Werkzeug**: A utility library for handling passwords securely.
- **CS50 Library**: A library for interacting with the SQLite database.

### Setup and Execution

1. **Installation**:

- Install the required dependencies using `pip`:

```bash

pip install flask flask-session
pip install cs50

```

2. **Running the Application**:

- Run the Flask application:

```bash

flask run

```

3. **Accessing the App**:

- Open a web browser and navigate to `http://localhost:5000` to access the application.

### Functionalities

**User Registration:**

- Users can register by providing a username and password.
- Passwords are securely hashed before storing in the database.

**User Login:**

- Registered users can log in with their credentials.
- Passwords are securely compared using hashed values.

**Session Management:**

- User sessions are managed using Flask-Session to keep users logged in.

**Authentication Decorator:**

- The login_required decorator is used to restrict access to certain routes, ensuring users are logged in.

**Error Handling:**

- Custom apology function renders appropriate error messages.

## Usage

1. **Homepage:**

- Access the homepage by visiting /.
- Only accessible to logged-in users.

2. **Login:**

- Access the login page by visiting /login.
- Provide a username and password to log in.

3. **Logout:**

- Access the logout functionality by visiting /logout.

4. **Registration:**

- Access the registration page by visiting /register.
- Provide a username and password to register a new account.

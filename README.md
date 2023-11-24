# Authentic App

This is a simple user authentication system built with Flask, utilizing HTML templates and form validation. The system includes features such as user registration, login, logout, and a basic dashboard.

## Prerequisites

Make sure you have the following dependencies installed:

- Flask
- Flask-SQLAlchemy
- Flask-Login
- Flask-WTF
- Flask-Bcrypt

You can install these dependencies using:

```bash
pip install flask flask_sqlalchemy flask_login flask_wtf flask-bcrypt
```

## Getting Started

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/flask-user-authentication.git
    ```

2. Navigate to the project directory:

    ```bash
    cd Authentic-App
    ```

3. Run the application:

    ```bash
    python app.py
    ```

4. Open your web browser and go to [http://127.0.0.1:5000/](http://127.0.0.1:5000/) to access the application.

## Project Structure

- **app.py**: The main Flask application file containing the routes and configurations.
- **templates**: This directory contains HTML templates for the home page, login page, signup page, and dashboard.
- **static**: This directory contains css files for the home page, login page, signup page, and dashboard.
- **database.db**: SQLite database file to store user information.

## Configuration

- `SQLALCHEMY_DATABASE_URI`: Database URI. This project uses SQLite, and the database file is named `database.db`.
- `SECRET_KEY`: Secret key for securing the application. Replace 'thisisasecretkey' with a strong secret key in production.

## User Model

The `User` class in the `app.py` file represents the model for the users in the database. It includes fields such as `id`, `username`, and `password`.

## Forms

- **SignupForm**: Form for user registration. It includes fields for `username`, `password`, and a submit button.
- **LoginForm**: Form for user login. It includes fields for `username`, `password`, and a submit button.

## Routes

- **/home**: Home page route, renders the home.html template.
- **/signup**: User registration route, renders the signup.html template. Handles user registration and password hashing.
- **/login**: User login route, renders the login.html template. Handles user authentication and login.
- **/dashboard**: Dashboard route, renders the dashboard.html template. Requires user authentication.
- **/logout**: Logout route, logs the user out and redirects to the login page.

## Contributing

Feel free to contribute to the development of this project by opening issues or submitting pull requests.

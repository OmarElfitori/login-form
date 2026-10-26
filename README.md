# login-form

A simple Java login form with input validation, hard-coded users, role verification, and a maximum login attempt limit.

## 📌 Project Overview

This project implements a basic desktop login form using **Java AWT/Swing**.

The application validates the user's input, checks the entered credentials against a list of hard-coded users, and displays appropriate messages when the login information is invalid.

## ✨ Features

- Username and password validation
- Prevents login when required fields are empty
- Hard-coded users using the `loadUsers()` method
- Username verification
- Password verification
- Role verification
- Clear error messages for invalid login information
- Maximum of **3 failed login attempts**
- Login button is disabled after 3 failed attempts
- Welcome page displayed after successful login

## 👤 Test Users

| Username | Password | Role |
|----------|----------|------|
| Ahmed | 1234 | Student |
| Ali | 5678 | TA |
| Mohamed | 9999 | Professor |

## 🔐 Validation

### Empty Fields

If the username or password is empty, the application displays:

> Please fill in all fields!

### Invalid Login

If the username, password, or selected role is incorrect, the application displays an error message and shows the number of remaining attempts.

### Failed Attempts Limit

The application allows a maximum of **3 failed login attempts**.

After the third failed attempt, the Login button is disabled and the following message is displayed:

> Too many failed attempts. Login is now disabled.

## ✅ Successful Login

When the entered username, password, and role match a valid user, the application opens a Welcome page displaying the user's username and role.

## 🛠️ Technologies Used

- Java
- Java AWT
- Java Swing
- `ArrayList` for storing users

## ▶️ How to Run

Make sure Java JDK is installed on your computer.

Compile the project:

```bash
javac LoginFormTask.java
```

Run the application:

```bash
java LoginFormTask
```

## 📸 Screenshots

Screenshots demonstrating the application's functionality and validation cases are included in the repository.

Recommended test cases:

1. Successful login
2. Empty username/password validation
3. Invalid credentials
4. Login disabled after 3 failed attempts

## 📁 Project Structure

```text
login-form/
│
├── LoginFormTask.java
├── README.md
└── screenshots/
    ├── successful-login.png
    ├── empty-fields.png
    ├── invalid-login.png
    └── three-failed-attempts.png
```

## 👨‍💻 Author

**Omar Elfitori**

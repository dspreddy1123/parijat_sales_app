# Sales Management App

Drrive link for Flutter Code :- https://drive.google.com/file/d/1t4SnRTc9cs9OkExc_2wcjXb4glopPki6/view?usp=sharing

This project is a comprehensive solution for managing sales, expenses, attendance, and other related functionalities. It consists of a Flutter-based mobile application integrated with a Flask backend. The app allows users to log in, submit orders, log expenses, mark attendance, and view reports.

## Table of Contents

- [Prerequisites]
- [Setting Up the Backend] 
- [Setting Up the Flutter App]
- [Project Structure]
- [Features]
- [Contributing]
- [License]
- [Contact]

## Prerequisites

Before you begin, ensure you have met the following requirements:

- **Flutter SDK**: Make sure you have Flutter installed. You can install it from (https://flutter.dev/docs/get-started/install).
- **Dart SDK**: Flutter uses Dart, so make sure you have Dart installed as well.
- **Python**: Ensure you have Python 3.13.0 installed.
- **MySQL**: Set up a MySQL database and configure the connection details in the Flask backend.

## Setting Up the Backend

1. **Install Python Dependencies**:
   ```bash
   pip install flask mysql-connector-python
   ```

2. **Database Setup**:
   - Create a MySQL database named `sales`.
   - Create the necessary tables by running the SQL scripts provided in the `database_scripts` directory.

3. **Configure Database Connection**:
   - Open the `app.py` file and update the `db_config` dictionary with your MySQL database credentials.

4. **Run the Flask Server**:
   ```bash
   python app.py
   ```
   The server will run on `http://192.168.1.138:5000`.

## Setting Up the Flutter App

1. **Navigate to the Flutter Project Directory**:
   ```bash
   cd <flutter-project-directory>
   ```

2. **Install Flutter Dependencies**:
   ```bash
   flutter pub get
   ```

3. **Update API Endpoint**:
   - Open the Flutter project and navigate to the API call sections (e.g., `log_expense.dart`, `order_list.dart`, etc.).
   - Ensure the API endpoints match the Flask server's IP address and port.

4. **Run the Flutter App**:
   ```bash
   flutter run
   ```

## Project Structure

- **`app.py`**: The Flask backend application.
- **`main.dart`**: The main entry point of the Flutter application.
- **`screens/`**: Contains various screens of the Flutter app (e.g., `login_page.dart`, `home_page.dart`, `expense_list.dart`, etc.).
- **`models/`**: Contains data models (e.g., `products.dart`).
- **`database_scripts/`**: Contains SQL scripts to set up the MySQL database.

## Features

### Login
Users can log in using their credentials.

### Order Management
- **Submit Orders**: Users can submit new orders.
- **View Order History**: Users can view their order history.

### Expense Management
- **Log Expenses**: Users can log new expenses.
- **View Expense History**: Users can view their expense history.

### Attendance
- **Mark Attendance**: Users can mark their attendance.
- **View Attendance History**: Users can view their attendance history.

### Profile
Users can view and edit their profile information.

### Settings
Users can configure app settings and log out.


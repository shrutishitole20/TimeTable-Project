📅 Timetabler - Academic Scheduling System

A full-stack web application built to automate, manage, and generate academic timetables efficiently. This system allows administrators to seamlessly manage university resources like tutors, rooms, courses, and lectures, and automatically generates conflict-free, print-ready weekly timetables.

✨ Features

🔐 Secure Authentication: User login and registration using industry-standard JWT (JSON Web Tokens).

📊 Interactive Dashboard: A clean, modern UI to navigate through different management modules.

👩‍🏫 Resource Management (CRUD):

Add, Edit, and Delete Tutors

Manage Courses and Departments

Manage Rooms and their capacities

Schedule Lectures and assign them to specific tutors and rooms

⚙️ Customizable Settings: Configure lecture durations and break times.

🗓️ Automated Timetable Generation: Automatically compiles all data into a beautiful weekly grid.

🖨️ Print-Ready: Built-in print functionality to easily export timetables to PDF or paper.

🛠️ Tech Stack

Frontend:

React.js

Axios (for API requests)

Vanilla CSS (Custom modern UI)

Backend:

Python / Django

Django REST Framework (DRF)

SimpleJWT (for secure token authentication)

Django CORS Headers

Database:

MySQL (MySQL Workbench)

🚀 Installation & Setup

Follow these steps to run the project locally on your machine.

Prerequisites

Node.js installed
*Python 3.x installed

MySQL Workbench installed

1. Database Setup

Open MySQL Workbench and run the following SQL command to create the database:

code
SQL
download
content_copy
expand_less
CREATE DATABASE timetable_db;
2. Backend Setup (Django)
Open your terminal, navigate to the backend folder, and run the following commands:
code
Bash
# Create and activate a virtual environment (optional but recommended)
python -m venv venv
venv\Scripts\activate  # On Windows
# source venv/bin/activate  # On Mac/Linux

# Install required Python packages
pip install django djangorestframework djangorestframework-simplejwt mysqlclient django-cors-headers

# Make database migrations
python manage.py makemigrations
python manage.py migrate

# Start the Django development server
python manage.py runserver
The backend will be running at http://127.0.0.1:8000
3. Frontend Setup (React)
Open a new terminal window, navigate to your frontend folder, and run:
code
Bash
# Install Node modules
npm install

# Start the React development server
npm start
The frontend will automatically open in your browser at http://localhost:3000
📡 API Endpoints Overview
The Django backend exposes the following RESTful APIs:
Authentication: /api/login/, /api/signup/, /api/logout/
Tutors: /api/tutors/
Courses: /api/courses/
Rooms: /api/rooms/
Lectures: /api/lectures/
Timetable: /api/timetable-slots/
Settings: /api/settings/
📸 Screenshots
(screenshots)
Dashboard:
Timetable View:
Login Page:<img width="1898" height="869" alt="image" src="https://github.com/user-attachments/assets/a8c19807-1e36-44d0-b59c-d9876cd7adeb" />




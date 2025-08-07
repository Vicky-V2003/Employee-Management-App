Employee Management System (Flask + MySQL)

A web-based Employee Management System built with **Flask** for the backend and MySQL for the database, with a dynamic HTML/CSS/JavaScript frontend. Users can perform Create, Read, Update, and Delete (CRUD) operations with inline editing and real-time updates.

##  Features

- **Add** new employee records via a separate form screen  
- **View** all employee details in a dynamic table  
- **Update** employee details inline with "Save" and "Cancel" actions  
- **Delete** employees with a confirmation prompt  
- **Form validation** for phone (numeric only, 10 digits) and email  
- **Duplicate prevention** by checking Name+Dept, Email, or Phone before Save

##  Tech Stack

- **Backend:** Python (Flask)  
- **Database:** MySQL  
- **Frontend:** HTML, CSS, JavaScript (Vanilla)  
- **Tools:** MySQL Workbench, Postman (for testing APIs)

##  Project Structure

Employee-Management-App/
├── backend/
│   └── app.py         # Flask backend API
├── frontend/
│   ├── index.html     # Main UI
│   ├── style.css      # Stylesheet
│   └── script.js      # Frontend logic
├── db.py              # Database connection helper
└── README.md

##  Getting Started

### Backend

1. Create MySQL database and table:

   CREATE DATABASE employee_management;
   USE employee_management;
   CREATE TABLE employees (
     id INT AUTO_INCREMENT PRIMARY KEY,
     name VARCHAR(100),
     dept VARCHAR(100),
     email VARCHAR(100) UNIQUE,
     phone VARCHAR(10) UNIQUE
   );

2. Configure your `db.py` credentials
   
3. Install dependencies and run the backend:
 Backend runs on `http://127.0.0.1:3000`.

### Frontend
* Open `frontend/index.html` in your browser.
* Ensure backend is running to handle API requests.





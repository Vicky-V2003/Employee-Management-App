🧑‍💼 Employee Management System (Flask + MySQL)

A simple Employee Management web application built using **Flask (Python)** for the backend and **HTML, CSS, JavaScript** for the frontend. The app allows you to create, read, update, and delete employee records stored in a **MySQL** database.

## 📁 Features

- Add new employees
- View all employees
- Update employee records inline
- Delete employee records with confirmation
- Form validations (email, phone number)
- Connected to MySQL backend using Flask
- Structured UI with separate screens for Create and Manage

---

## 🧩 Technologies Used

- **Frontend**: HTML, CSS, JavaScript  
- **Backend**: Flask (Python)  
- **Database**: MySQL  
- **Tools**: MySQL Workbench, VS Code  

---

## 🛠️ Setup Instructions

### 1. 🔁 Clone the Repository

```bash
git clone https://github.com/Vicky-V2003/Employee-Management-App.git
cd Employee-Management-App
````

---

### 2. 📦 Set Up Python Environment

```bash
# Create virtual environment (optional)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install required packages
pip install -r requirements.txt
```

If `requirements.txt` is missing:

```bash
pip install flask flask-mysqldb flask-cors
```

---

### 3. 🧮 Set Up MySQL Database

1. Open **MySQL Workbench**
2. Create a database named `employee_db`
3. Run:

```sql
CREATE TABLE employees (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(100),
  email VARCHAR(100),
  phone VARCHAR(15),
  department VARCHAR(100)
);
```

Make sure the database credentials in `app.py` match your local setup:

```python
app.config['MYSQL_HOST'] = 'localhost'
app.config['MYSQL_USER'] = 'your_username'
app.config['MYSQL_PASSWORD'] = 'your_password'
app.config['MYSQL_DB'] = 'employee_db'
```

---

### 4. ▶️ Run the Flask Server

```bash
python app.py
```

> Server will start at: `http://localhost:3000`

---

### 5. 🌐 Open the Frontend

Open `index.html` in a browser, or use the **Live Server** extension in VS Code.

      **Ensure API requests point to: `http://localhost:3000`**











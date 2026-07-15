# 📊 Personal Finance Tracker

A sleek, full-stack **Personal Finance Tracker** built with Python (Flask), MySQL, and Chart.js. This application is designed to help users take complete control of their financial health through secure login, real-time transaction tracking, dynamic budgeting, and interactive visual analytics.

---

## 🚀 Features

*   **🔐 Secure Account Authentication:** A modern, sleek login screen ensuring your financial data is safely sandboxed to your private account.
*   **📈 Interactive Dashboard:** Instantly view your overall financial health (**Total Income**, **Total Expenses**, and **Net Balance**) with real-time visual charts (using `Chart.js`).
*   **➕ Transaction Logging:** Easily record incoming and outgoing cash flows, complete with categories, descriptions, and custom dates.
*   **💰 Smart Budgeting:** Set monthly, category-specific budget limits. Visual progress bars dynamically turn amber or red as you approach your limits.
*   **🎯 Savings Goals:** Define savings targets with custom deadlines and visually add money over time until your goal is 100% complete.

---

## 🛠️ Tech Stack

*   **Frontend:** Vanilla HTML5, CSS3, JavaScript, Chart.js (for analytics).
*   **Backend:** Python 3.13, Flask (RESTful API).
*   **Database:** MySQL, Flask-SQLAlchemy (ORM).

---

## 📦 Installation & Setup

Follow these steps to get the application running locally on your machine:

### Prerequisite: MySQL Setup
1. Open your MySQL client (Terminal or MySQL Workbench).
2. Create the project database:
   sql
   CREATE DATABASE personal_finance_db;

   git clone [https://github.com/YOUR_USERNAME/personal-finance-tracker.git](https://github.com/YOUR_USERNAME/personal-finance-tracker.git)
cd personal-finance-tracker

# Create and activate virtual environment
python -m venv venv
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate

pip install Flask flask-sqlalchemy pymysql cryptography python-dotenv

db_user = 'root'
db_password = 'YourMySQLPassword'  # Leave blank '' if no password is set
db_host = 'localhost'
db_name = 'personal_finance_db'

python -c "from app import app, db; app.app_context().push(); db.create_all()"

python app.py

📓 Digital Diary : MINI PROJECT
A full-featured Digital Diary Web Application built with Flask, SQLAlchemy, and Bootstrap 5.
Designed as a practice project to demonstrate user authentication, CRUD operations, mood tracking, tagging, search functionality, and responsive design.

https://img.shields.io/badge/Flask-2.3.3-blue  
https://img.shields.io/badge/SQLAlchemy-3.0.5-red  
https://img.shields.io/badge/Bootstrap-5-purple  
https://img.shields.io/badge/license-MIT-green

✨ FEATURES
User Authentication – Registration, login, logout, password hashing, “Remember Me”

Diary Entries – Create, read, update, delete entries with rich text content

Mood Tracking – Choose mood (happy, excited, calm, sad, etc.) with emoji & color coding

Privacy Control – Mark entries as public or private

Tagging System – Add comma-separated tags, search by tags

Search – Find entries by title, content, or tags (public entries + your own)

Statistics Dashboard – See total entries, public/private split, mood distribution

User Profile – Account age, entry counts, last login tracking

Public Entries Feed – Explore recent public entries on the home page

REST API Endpoint – /api/stats returns global usage statistics (JSON)

Responsive UI – Works on desktop, tablet, and mobile (Bootstrap 5)

🛠️ Tech Stack
Layer	Technology
Backend	Flask (Python)
Database	SQLite + SQLAlchemy ORM
Authentication	Flask-Login + Werkzeug password hashing
Frontend	Bootstrap 5, HTML5, CSS3, Jinja2 templates
Icons	Emoji (mood indicators)


📁 PROJECT STRUCTURE
Code
digital-diary/
├── app.py                 # Main application
├── requirements.txt       # Dependencies
├── digital_diary.db       # SQLite database (auto-created on first run)
├── templates/             # HTML templates
│   ├── index.html
│   ├── login.html
│   ├── register.html
│   ├── dashboard.html
│   ├── add_entry.html
│   ├── view_entry.html
│   ├── search.html
│   ├── profile.html
│   ├── 404.html
│   └── 500.html
├── static/
│   └── style.css
└── README.md
Note: The templates and static folders are required for the app to run. If missing, create them based on the routes defined in app.py.

🚀 START GETTING
Prerequisites
Python 3.8 or higher

pip (PYTHON PACKAGE MANAGER)

Installation
bash
# Clone the repository
git clone https://github.com/your-username/digital-diary.git
cd digital-diary

# Create a virtual environment (recommended)
python -m venv venv
source venv/bin/activate   # On Linux/Mac
venv\Scripts\activate      # On Windows

# INSTALL DEPENDENCIES
pip install -r requirements.txt

# RUN THE  APPLICATIONS
python app.py
On first run, the script will:

Create digital_diary.db (SQLite database)

Create all tables (User, DiaryEntry)

Populate sample data (demo user, admin user, and 4 sample entries)

Open your browser at: http://localhost:5000

🔐 Demo Credentials
Role	Username	Password
Student	demo_student	password123
Admin	admin	admin123


You can also register a new account from the login page.

📚 USAGE GUIDE
Dashboard – View all your diary entries, filter by mood, 

Add Entry – Write a new diary entry, choose mood, set privacy, add tags

Edit/Delete – Manage your own entries

Search – Find entries by title, content, or tags

Profile – View account info and overall statistics

Logout – Securely log out from the navbar

Public Area (not logged in):

See recent public entries on the home page

View individual public entries 

🌐 API Endpoint
URL: /api/stats

Method: GET

Response Example:

json
{
  "total_users": 2,
  "total_entries": 5,
  "public_entries": 3,
  "database": "SQLite",
  "status": "online",
  "timestamp": "2025-01-29T12:34:56"
}
🧪 Running in Production (Optional)
For deployment, set environment variables:

bash
export SECRET_KEY="your-random-secret-key"
export FLASK_ENV="production"
Modify app.py to read from os.environ.get() and set debug=False.

📸 Screenshots


Home Page → https://screenshots/home.png

Dashboard → https://screenshots/dashboard.png

Add Entry → https://screenshots/add.png



🤝 Contribution
Suggestions and improvements are welcome!


📄 License
This project is open-source and available under the MIT License.

📬 Contact
Author: Shreekanth A Guttedar

GitHub: shreekanthashokg-lang (github.com in Bing)

Email: 2222509208@svysa-sas.edu.in




📓 DIGITAL DIARY : MINI PROJECT
A FUL-featured digital diary Web APPLICATION BUILT WITH FLASK,SQLAlchemy and Bootstrap 5.
Designed as A PRATICE project to demonstrate user authentication, CRUD operations, mood tracking, tagging, and responsive design.


│   └── 500.html
├── static/
│   └── style.css
└── README.md
NOTE: The templates and static folder are required for the app to run.
If they are missing, you can create them based on the routes defined in app.py.

🚀 GETTING STARTED
PREREUISITES 
PYTHON 3.8 or HIGHER

pip (Python package manager)

INSTALLATION
CLONE THE REPOSITORY

bash
git clone https://github.com/your-username/digital-diary.git
cd digital-diary
Create a virtual environment (recommended)

bash
python -m venv venv
source venv/bin/activate      
Install dependencies

bash
pip install -r requirements.txt
Run the application

bash
python app.py
On first run, the script will:

Create digital_diary.db (SQLite database)

CREATE ALL tables (User, DiaryEntry)

Populate sample data (demo user, admin user, and 4 sample entries)

OPEN YOUR BROWSER :
http://localhost:5000

🔐 DEMO CREDENTIALS
USE THESE ACCOUNTS TO TEST THE APPLICATION IMMEDIATELY :

ROLE	Username	Password
Student (Demo)	demo_student	password123
Admin	admin	admin123
You can also register a new account from the login page.

📚 USAGE GUIDE
After logging in
Dashboard – View all your diary entries, filter by mood, see statistics.

ADD ENTRY – Write a new diary entry, choose mood, set privacy, add tags.

Edit/Delete – Each entry has edit/delete buttons (only for your own entries).

Search 
Profile – View your account info and overall statistics.

Logout – Click the logout button in the navbar.

Public area (not logged in)
See recent public entries on the home page.

View individual public entries (private entries are hidden).


API ENDPOINT
URL: /api/stats

METHOD: GET

RESPONSE EXAMPLE:

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
The current configuration uses debug=True and a hardcoded SECRET_KEY, which is fine for development/demonstration.
For a real deployment, set the following environment variables:

bash
export SECRET_KEY="your-random-secret-key"
export FLASK_ENV="production"
Then modify app.py to read from os.environ.get() and set debug=False.

📸 Screenshots
(Add actual screenshots of your running app here)

HOME PAGE	Dashboard	Add Entry
https://screenshots/home.png	https://screenshots/dashboard.png	https://screenshots/add.png
🧰 Customization
Add more moods – Edit get_mood_emoji() and get_mood_color() in app.py.

Change database – 


🤝 MY CONTRIBUTION
suggestions and improvements are welcome!

📄 License
This project is open-source and available under the MIT License.

📬 Contact:
Project Author –Student
SHREEKANTH A GUTTEDAR
GitHub: https://github.com/shreekanthashokg-lang
Email:  2222509208@svysa-sas.edu.in
Email:  shreekanthashokg@gmail.com

# Task 4 – Flask + MongoDB (Form)

Simple app to submit task details and save them to MongoDB.

## Requirements
- Python 3.8+
- MongoDB Community Server (local)
- Git (optional, for cloning)

## Run (Windows)
```powershell
# Start MongoDB (keep this terminal open)
mongod --dbpath "D:\AI_TASK\mongo-data"

# New terminal in the project folder
.\venv\Scripts\Activate.ps1
pip install -r requirements.txt
.\venv\Scripts\python.exe app.py
Open: http://127.0.0.1:5000


Verify data (CLI)
mongosh
use task_manager
db.submitted_tasks.find().sort({_id:-1}).limit(1)


Project structure
task1_form/
  app.py
  db.py
  requirements.txt
  static/      # frontend JS
  templates/   # HTML







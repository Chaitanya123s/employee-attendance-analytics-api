Employee Attendance & Analytics API

This project is a REST API developed using Python, FastAPI, and MongoDB. It manages employee details and attendance records through API endpoints.

Features

- Create and manage employee records
- Record employee punch-in details
- Store attendance data in MongoDB
- Test API endpoints using Swagger UI
- Configure database settings through environment variables

Technologies Used

- Python
- FastAPI
- MongoDB
- PyMongo
- Pydantic
- Uvicorn

Project Structure

candidate_kit/
├── app/
│   ├── __init__.py
│   └── main.py
├── sample_data/
│   ├── employees.json
│   └── attendance_logs.json
├── sample_seed.py
├── requirements.txt
├── openapi.yaml
├── DATA_MODEL.md
├── DECISIONS.md
└── PROBLEM_STATEMENT.docx

How to Run the Project

1. Clone the repository

git clone https://github.com/Chaitanya123s/employee-attendance-analytics-api.git
cd employee-attendance-analytics-api/candidate_kit

2. Create a virtual environment

python -m venv venv

Activate it in Windows PowerShell:

.\venv\Scripts\Activate.ps1

3. Install the required packages

pip install -r requirements.txt

4. Configure MongoDB

Create a local ".env" file and add your database configuration:

MONGO_URI=mongodb://localhost:27017
MONGO_DB=your_database_name

Make sure MongoDB is running before starting the application.

5. Start the API

Run this command from the "candidate_kit" directory:

uvicorn app.main:app --reload

6. Test the API

Open the following URL in your browser to access the interactive API documentation:

http://127.0.0.1:8000/docs

Security

The ".env" file contains local configuration and should not be uploaded to GitHub. Keep database credentials and other sensitive information private.

About

This project was developed as part of an employee attendance and analytics API assignment.

DemoBank QA Audit Submission
Tester : Divyasri

Project Overview : This project contains functional testing performed on the DemoBank application as part of the CDF Agentic QA Hackathon.

Environment Setup :
Backend -

Navigate to:
cd test-website/backend

Activate virtual environment:
.\.venv\Scripts\Activate.ps1

Run backend:
uvicorn demobank.main:app --host 0.0.0.0 --port 8000 --reload

Backend Health Check:
http://localhost:8000/health

Frontend -
Navigate to:
cd test-website/frontend

Run frontend:
npm run dev

Frontend URL:
http://localhost:5173

Database :
Docker Compose -
cd test-website/database

docker compose up -d

Application URLs :
Frontend -
http://localhost:5173

Backend Health -
http://localhost:8000/health

Test Results
Total Tests Executed: 27
Passed: 25
Failed: 2
Defects found: 2
Pass Rate: 92.59%

Modules Tested
Authentication
Accounts
Transfers
Transaction History
Profile

Defects Found :
BUG-001 -
Zero amount transfer accepted.
Severity: Medium

BUG-002 -
Negative amount transfer accepted.
Severity: High

Documentation :
bug_report.md
test_execution_summary.md

Walkthrough Video :
Paste your Google Drive video link here after upload.

Example:

https://drive.google.com/xxxxx

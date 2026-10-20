# QR-Based Student Attendance Management System

A web-based student attendance management system built using Python, Flask, SQLite, JavaScript and QR-code scanning. The project digitises attendance recording and provides a structured way to manage student information, attendance sessions, grades and schedules.

## Project Overview

Traditional attendance registers can require manual record-keeping and make attendance information harder to organise and review. This project provides a web-based approach to recording attendance through QR-code scanning and managing related academic information.

The application combines a Flask backend, an SQLite database and a browser-based interface for attendance management.

## Key Features

- **QR-Code Attendance:** Supports QR-code-based attendance recording through a browser-based scanning interface.
- **Student Management:** Stores and manages student records.
- **Attendance Sessions:** Supports the management of attendance sessions.
- **Attendance Records:** Maintains attendance information associated with students and sessions.
- **Authentication:** Includes an authentication mechanism for access to the application.
- **Attendance Validation:** Applies validation during attendance recording to help maintain data consistency.
- **Academic Information:** Supports the management of student grades and schedules.
- **Attendance Reporting:** Provides attendance reports and summary queries for student-level monitoring.
- **SQLite Database:** Uses a lightweight relational database to store application data.

## Technology Stack

| Technology | Purpose |
|---|---|
| Python | Backend programming |
| Flask | Web application framework |
| SQLite | Relational database |
| HTML5 | Web page structure |
| JavaScript | Browser-side functionality |
| HTML5 QR Code | QR-code scanning in the browser |
| qrcode | QR-code generation in Python |

## Project Architecture

The application follows a simple web application architecture.

1. **Frontend:** HTML templates and JavaScript provide the user interface and QR-scanning functionality.
2. **Backend:** Flask handles application requests and server-side processing.
3. **Database layer:** SQLite stores student, session, attendance and related academic records.
4. **QR utilities:** QR-code functionality supports attendance session creation and scanning workflows.
5. **Attendance utilities:** Attendance-processing functionality validates and records attendance.
6. **Reporting:** Database queries support attendance summaries and student-level monitoring.

## Suggested Project Structure

The following is a suggested repository structure. Retain the actual filenames and folders from your implementation.

```text
QR-Based-Student-Attendance-System/
│
├── app.py
├── utils/
│   ├── db.py
│   ├── qr_utils.py
│   └── attendance_utils.py
│
├── templates/
│   └── [your HTML templates]
│
├── static/
│   ├── css/
│   ├── js/
│   └── images/
│
├── requirements.txt
├── .gitignore
└── README.md
```

## Installation and Setup

### Prerequisites

- Python 3.10 or a compatible version supported by your dependencies
- pip
- Git
- A modern web browser with camera access for QR scanning

### 1. Clone the repository

```bash
git clone https://github.com/anoopnaveen10/QR-Based-Student-Attendance-System.git
cd QR-Based-Student-Attendance-System
```

### 2. Create a virtual environment

Windows:

```bash
python -m venv venv
venv\Scripts\activate
```

macOS or Linux:

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure the application

Check the application source code for its required environment variables, database initialisation steps and configuration settings.

Do not upload passwords, secret keys or private configuration files.

### 5. Initialise the database

Follow the database initialisation procedure implemented in the project. The database setup should create or prepare the tables required by the application.

### 6. Run the application

If the Flask application entry point is `app.py`, try:

```bash
python app.py
```

Otherwise, use the entry point and run command defined in your implementation.

Open the local URL displayed in the terminal.

> **Note:** These instructions assume the filenames and commands shown match your actual source code. Update them if your implementation differs.

## How the System Works

The intended attendance workflow is:

1. The authorised user accesses the application.
2. An attendance session is created.
3. A QR code is generated for the session.
4. A student scans the QR code using the browser-based scanner.
5. The application validates the attendance request.
6. The attendance record is processed and stored in the database.
7. Attendance records and summaries can be reviewed through the application's reporting functionality.

The exact validation rules and session behaviour depend on the implementation in the source code.

## Database Overview

The database supports the following categories of information:

- **Students:** Student-related records.
- **Sessions:** Attendance session information.
- **Attendance:** Records associated with attendance activity.
- **Grades:** Student academic grade information.
- **Schedules:** Student schedule information.

These describe the project's data categories; the exact table names, columns, relationships and constraints should be documented from the actual SQLite schema.

## Testing Checklist

Use this checklist when verifying the application:

- [ ] Confirm that authorised users can access the application.
- [ ] Verify that an attendance session can be created.
- [ ] Verify that the QR code can be displayed and scanned.
- [ ] Confirm that valid attendance requests are recorded correctly.
- [ ] Test invalid QR codes and expired sessions if expiry validation is implemented.
- [ ] Check whether repeated scans are rejected if duplicate-scan prevention is implemented.
- [ ] Verify that attendance records can be retrieved.
- [ ] Check that attendance reports return the expected information.
- [ ] Confirm that student grades and schedules are handled correctly.

Only mark tests as completed after running them.

## Security and Privacy

- Do not commit passwords, secret keys or API credentials.
- Do not upload a production database containing identifiable student information.
- Use synthetic or anonymised data for demonstrations.
- Configure production secrets through environment variables.
- Verify access controls and attendance validation before deploying the application publicly.

## Future Improvements

Potential extensions, if implemented in the future, include:

- Attendance analytics dashboards.
- Exportable attendance reports.
- Improved role-based access controls.
- Automated testing and continuous integration.
- Integration with business intelligence tools such as Power BI.

These are possible future enhancements, not claims about existing functionality.

## Skills Demonstrated

- Python application development
- Flask web development
- Relational database management
- SQL and data retrieval
- QR-code integration
- Input validation and data consistency
- Attendance reporting
- Software project organisation

## Author

**Anoop Naveen**

GitHub: https://github.com/anoopnaveen10

LinkedIn: https://linkedin.com/in/anoopnaveen10

## Disclaimer

This project is intended for educational and portfolio purposes. Any demonstration data should be synthetic or appropriately anonymised.

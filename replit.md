# Student Portal - Django Web Application

## Overview
This is a Django-based student portal application that allows management of students, workshops, marks, and certifications. The application has been successfully imported and configured for the Replit environment.

## Recent Changes
- **September 04, 2025**: Successfully imported from GitHub and configured for Replit
  - Installed Python 3.11 and all required dependencies
  - Configured Django settings for Replit proxy support (ALLOWED_HOSTS)
  - Set up database migrations and static files
  - Configured development server on port 5000
  - Set up production deployment with gunicorn

## Project Architecture

### Technologies Used
- **Backend**: Django 5.2.6 with Python 3.11
- **Database**: SQLite3 (development), PostgreSQL support configured
- **Static Files**: WhiteNoise for static file serving
- **Data Import/Export**: django-import-export with Excel/CSV support
- **Data Processing**: pandas, openpyxl for data handling

### Key Features
- Student management system
- Workshop management
- Attendance tracking
- Marks/grades management
- Certification upload system
- Bulk data import/export capabilities
- Admin dashboard

### Directory Structure
```
├── student_portal/          # Django project settings
├── portal_app/             # Main application
│   ├── templates/          # HTML templates
│   ├── static/            # CSS, images, JS
│   ├── migrations/        # Database migrations
│   └── models.py          # Data models
├── media/                 # User uploaded files
├── static/               # Collected static files
├── staticfiles/          # Production static files
└── db.sqlite3           # SQLite database
```

### Configuration
- **Development Server**: Runs on 0.0.0.0:5000
- **Production Deployment**: Configured with gunicorn on autoscale
- **Static Files**: Handled by WhiteNoise middleware
- **Database**: Uses dj-database-url for flexible database configuration

## Current Status
✅ Fully functional and ready for use
✅ Development server running on port 5000
✅ Production deployment configured
✅ All dependencies installed and working
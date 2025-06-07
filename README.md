# Job Board Application

A modern, responsive job board application built with Django that allows users to post jobs, apply for positions, and manage their applications.

## Features

### For Job Seekers
- User registration, login, logout, and profile management
- Browse and search jobs with advanced filters
- Save interesting jobs for later
- Apply to jobs with resume upload
- Track application status (Pending, Accepted, Rejected)
- View application history and statistics
- Receive email notifications for application updates

### For Admin
- Create and manage company profiles
- Post, update, and delete job listings
- Review and manage job applications
- Update application statuses
- Send email notifications to applicants
- View detailed application statistics
- Manage multiple companies and their profiles
- Control job categories and tags
- Access comprehensive admin dashboard
- Monitor and moderate user accounts
- Generate reports and analytics

### General Features
- Responsive design for desktop, tablet, and mobile devices
- User authentication and authorization
- Email notifications
- Advanced search and filtering
- Job categories and tags
- Company profiles
- Admin dashboard

## Technical Stack

- **Backend:** Django 4.2.7
- **Frontend:** HTML5, CSS3, JavaScript, Bootstrap 5, Font Awesome, Custom CSS and JS
- **Database:** SQLite (development)
- **Email:** SMTP (Gmail)
- **Additional Packages:** python-dotenv, Pillow, django-crispy-forms

## Installation and Setup

### Prerequisites
- Python 3.8 or higher
- pip (Python package manager)
- Git

### Steps

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd job-board
   ```

2. Create and activate a virtual environment:
   ```bash
   # Windows
   python -m venv venv
   venv\Scripts\activate

   # Linux/Mac
   python3 -m venv venv
   source venv/bin/activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Create a `.env` file in the project root with the following variables:
   ```
   SECRET_KEY=your-secret-key
   DEBUG=True
   EMAIL_HOST_USER=your-email@gmail.com
   EMAIL_HOST_PASSWORD=your-app-password
   DEFAULT_FROM_EMAIL=your-email@gmail.com
   ```

5. Run migrations:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

6. Create a superuser:
   ```bash
   python manage.py createsuperuser
   ```

7. Run the development server:
   ```bash
   python manage.py runserver
   ```

8. Visit `http://127.0.0.1:8000` in your browser

## Project Structure

```
job_board/
├── job_board/          # Project settings
├── jobs/               # Jobs app
├── applications/       # Applications app
├── accounts/           # User management app
├── templates/          # HTML templates
├── static/             # Static files (CSS, JS, images)
└── media/              # User-uploaded files
```

## Database Models Overview

- **User & Profile:** Extended user model with profile details including resume, company info, and image.
- **Job:** Job postings with details like title, description, company, category, location, salary, and status.
- **Application:** Job applications linked to jobs and users, with status tracking and admin notes.
- **Company:** Company profiles with logo, website, and location.
- **Category:** Job categories for organizing job listings.
- **JobApplication & SavedJob:** Additional models for managing applications and saved jobs.

## Security Features

- CSRF protection
- XSS prevention
- Secure password handling
- Environment variable configuration
- File upload validation
- User authentication and authorization

## Responsive Design

- Mobile-first approach using Bootstrap 5 grid system
- Custom responsive CSS and flexible layouts
- Optimized images and touch-friendly interface

## Email Notifications

- Application status updates
- Job posting confirmations
- Password reset emails
- Welcome emails with custom templates

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support

For support, email [your-email@example.com] or create an issue in the repository.

## Acknowledgments

- Django Documentation
- Bootstrap Documentation
- Contributors and maintainers
- Open source community

## Copyright

© 2025 MISHECK MAWERE M241135. All rights reserved.

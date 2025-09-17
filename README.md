# Django Blog Application

A simple blog application built with Django for learning and local development.

## Features

- Create and manage blog posts
- User registration and authentication
- Comment on posts
- User profiles with profile pictures
- Tag system for organizing posts
- Admin panel for content management

## Local Development Setup

### Prerequisites
- Python 3.8 or higher ([Download from python.org](https://www.python.org/downloads/))
- pip (comes with Python)
- Command Prompt (Windows) or Terminal (Mac/Linux)

### Quick Start

1. **Navigate to the project directory**
   ```bash
   cd "django-blog app"
   ```

2. **Create and activate virtual environment**
   
   **On Windows:**
   ```cmd
   python -m venv venv
   venv\Scripts\activate
   ```
   
   **On Mac/Linux:**
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run database migrations**
   ```bash
   python manage.py migrate
   ```

5. **Create an admin user (optional)**
   ```bash
   python manage.py createsuperuser
   ```

6. **Start the development server**
   ```bash
   python manage.py runserver
   ```

7. **Open your browser**
   - Main site: http://127.0.0.1:8000/
   - Admin panel: http://127.0.0.1:8000/admin/

## Usage

- **Homepage**: View all blog posts
- **Register/Login**: Create an account to post blogs
- **Create Posts**: Write and publish your blog posts
- **Comments**: Leave comments on posts
- **Admin Panel**: Manage all content (if you created a superuser)

## Database

This project uses SQLite for local development - no additional database setup required!

## Troubleshooting

If you encounter issues:

1. **Virtual environment**: Make sure it's activated
   - Windows: `venv\Scripts\activate`
   - Mac/Linux: `source venv/bin/activate`
2. **Python command**: 
   - On Windows: use `python` instead of `python3`
   - On Mac/Linux: use `python3`
3. **Dependencies**: Try `pip install --upgrade pip` then reinstall requirements
4. **Migrations**: Run `python manage.py migrate` if you see database errors
5. **Port conflicts**: Use `python manage.py runserver 8080` to run on a different port

## Project Structure

```
django-blog app/
├── blog/           # Main Django settings
├── core/           # Blog posts, comments, tags
├── users/          # User authentication and profiles
├── templates/      # HTML templates
├── static/         # CSS, images, etc.
├── manage.py       # Django management commands
└── db.sqlite3      # Local database (created after first run)
```

## What's Included

- **Posts**: Title, content, images, tags
- **Users**: Custom user model with email login
- **Comments**: Simple commenting system
- **Profiles**: User profiles with bio and profile pictures
- **Admin**: Full Django admin interface

That's it! Happy blogging! 🚀
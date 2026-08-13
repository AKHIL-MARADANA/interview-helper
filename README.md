# Django Blog

A full-stack blog web application built using Django.

## Features

- User registration and login
- User profile
- Create blog posts
- View blog posts
- Update your own blog posts
- Filter posts by company
- User authentication and authorization

## Technologies Used

- Python
- Django
- SQLite
- HTML
- CSS
- Bootstrap
- django-crispy-forms
- python-dotenv

## Project Structure

```text
blog/
│
├── django_blog/
│   ├── blog/
│   ├── users/
│   ├── django_blog/
│   ├── manage.py
│   └── ...
│
├── requirements.txt
└── README.md
```

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/AKHIL-MARADANA/interview-helper.git
```

### 2. Navigate to the project

```bash
cd interview-helper/django_blog
```

### 3. Create a virtual environment

```bash
python -m venv venv
```

### 4. Activate the virtual environment

For Windows PowerShell:

```powershell
venv\Scripts\activate
```

### 5. Install dependencies

```powershell
python -m pip install -r ..\requirements.txt
```

## Environment Variables

Create a `.env` file inside the `django_blog` folder, in the same location as `manage.py`.

Add:

```text
SECRET_KEY=your-secret-key-here
```

Do not upload the `.env` file to GitHub.

## Database Setup

```powershell
python manage.py migrate
```

## Run the Application

```powershell
python manage.py runserver
```

Then open:

```text
http://127.0.0.1:8000/
```

## Main Functionality

### User Authentication

Users can:

- Register an account
- Log in
- Log out
- View their profile

### Blog Posts

Authenticated users can:

- Create blog posts
- View blog posts
- Update their own posts

Each post can contain:

- Title
- Company name
- Year
- Content
- Author
- Date posted

### Company Filtering

Users can filter blog posts based on the company associated with each post.

## Security

Sensitive configuration such as the Django `SECRET_KEY` is stored using environment variables rather than being directly included in the source code.

## Future Improvements

- Add post deletion
- Add comments
- Add pagination
- Add search functionality
- Add image upload support
- Improve UI/UX
- Deploy the application online
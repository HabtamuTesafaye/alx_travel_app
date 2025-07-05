```markdown
# alx_travel_app

A Django-based travel listing platform backend project.

This project demonstrates best practices for initializing a Django REST API backend with MySQL, environment variables management, CORS, and Swagger API documentation.

---

## Features

- Modular Django project structure with `listings` app
- MySQL database integration
- Environment variable management using `django-environ`
- Cross-Origin Resource Sharing (CORS) setup
- API documentation with Swagger (`drf-yasg`)

---

```
## Project Structure

``` 
alx_travel_app/
├── alx_travel_app/           # Django project folder
│  ├── listings/                 # Django app for travel listings
│  │   ├── __init__.py
│  │   ├── admin.py
│  │   ├── apps.py
│  │   ├── models.py
│  │   └── views.py
│  ├── __init__.py
│  ├── settings.py
│  ├── urls.py
│  ├── wsgi.py
|  └──requirements.txt   
├── manage.py                 # Django CLI       # Python dependencies
├── .env.example              # Sample environment variables file
├── README.md
└── venv/                    # Virtual environment (not committed)
```


````

---

## Getting Started

### Prerequisites

- Python 3.8+
- MySQL server installed and running
- Virtual environment tool (`venv` or similar)
- Git

---

### Installation Steps

1. **Clone the repository**

```bash
git clone https://github.com/yourusername/alx_travel_app.git
cd alx_travel_app
````

2. **Create and activate virtual environment**

```bash
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install dependencies**

```bash
pip install -r requirements.txt
```

4. **Create your own `.env` file**

Copy the sample `.env.example` and fill in your secrets:

```bash
cp .env.example .env
```

Edit `.env` with your actual secret values.

> **Note:** Do NOT commit `.env` to version control.

5. **Set up your MySQL database**

Make sure your MySQL server is running and create a database matching the name in `.env` (`alxtravel`):

```sql
CREATE DATABASE alxtravel;
```

6. **Run migrations**

```bash
python manage.py migrate
```

7. **Run the development server**

```bash
python manage.py runserver
```

8. **Access API documentation**

Visit [http://localhost:8000/swagger/](http://localhost:8000/swagger/) to see the Swagger UI for the API.

---



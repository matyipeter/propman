# 🧑‍💻 Django + Node.js Project

A well-structured Django project integrated with Node.js for frontend asset management, and Docker support for easy deployment.

## 📁 Project Structure

```
myproject/
├── manage.py            # Django project manager
├── venv/                # Virtual environment (excluded in .gitignore)
├── static/              # Static files (CSS, JS, images)
├── templates/           # HTML templates
├── myproject/           # Core Django settings
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
└── core/                # Main app
    ├── __init__.py
    ├── models.py
    ├── views.py
    ├── urls.py
    └── templates/core/
```

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/your-username/django-project.git
cd django-project
```

### 2. Set Up Virtual Environment
```bash
python -m venv venv
# Activate the virtual environment
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Environment Configuration
Create a `.env` file in the root directory:

```
DEBUG=True
SECRET_KEY=your-secret-key
DATABASE_URL=sqlite:///db.sqlite3
```

### 5. Run Migrations
```bash
python manage.py migrate
```

### 6. Run the Development Server
```bash
python manage.py runserver
```
Access the project at: [http://127.0.0.1:8000](http://127.0.0.1:8000)

## 📦 Node.js Integration
Ensure Node.js is installed:

```bash
node -v
npm -v
```

### 1. Install Frontend Packages
```bash
npm install
```

### 2. Build Frontend Assets
```bash
npm run build
```

## 🐳 Docker Setup (Optional)

1. Build Docker Image:
```bash
docker build -t django-node-project .
```

2. Run Docker Container:
```bash
docker-compose up
```

## ✅ Useful Commands

- Create Superuser:
  ```bash
  python manage.py createsuperuser
  ```

- Collect Static Files:
  ```bash
  python manage.py collectstatic
  ```

- Run Tests:
  ```bash
  python manage.py test
  ```

## 📜 License
This project is licensed under the MIT License. Feel free to use and modify it.

## 📧 Contributing
Feel free to submit issues or pull requests. We welcome contributions!

---
Made with ❤️ by [Your Name](https://github.com/your-username)



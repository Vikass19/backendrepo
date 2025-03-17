# Backendrepo

## Overview
This repository contains the backend APIs for a blog website, built using Django and Django Rest Framework (DRF). The backend is responsible for handling user authentication, blog management, comments, and categories. The project is hosted on **AWS Free Tier** and can be accessed via the following API endpoint:

🔗 **Live API URL:** [http://54.252.157.69/api/](http://54.252.157.69/api/)

## Features
- **User Authentication** (Register, Login, JWT Token-based Authentication)
- **Post Management** (Create, Read, Update, Delete Posts)
- **Categories & Filtering**
- **User Comments on Posts**
- **Secure API Endpoints with Permissions**

## Tech Stack
- **Django** (Backend Framework)
- **Django Rest Framework (DRF)** (API Development)
- **PostgreSQL/MySQL** (Database)
- **AWS Free Tier** (Hosting)
- **JWT Authentication** (Security)

## Installation & Setup
### 1. Clone the Repository
```bash
git clone https://github.com/Vikass19/backendrepo.git
cd backendrepo
```

### 2. Create Virtual Environment & Install Dependencies
```bash
python -m venv env
source env/bin/activate  # On Windows use: env\Scripts\activate
pip install -r requirements.txt
```

### 3. Configure Environment Variables
Create a `.env` file and add the necessary credentials:
```
SECRET_KEY=your_secret_key
DEBUG=True
DATABASE_URL=your_database_url
```

### 4. Apply Migrations
```bash
python manage.py migrate
```

### 5. Run the Development Server
```bash
python manage.py runserver
```
API will be available at: [http://127.0.0.1:8000/api/](http://127.0.0.1:8000/api/)

## API Endpoints
| Endpoint | Method | Description |
|----------|--------|-------------|
| `/api/posts/` | GET | Get all posts |
| `/api/posts/<id>/` | GET | Get a single post |
| `/api/comments/` | GET, POST | Get all comments / Add a comment (Authenticated) |
| `/api/user-profile/` | GET | Get user profile |
| `/api/categories/` | GET | Get all categories |

## Deployment on AWS
This project is deployed on **AWS Free Tier** using **EC2** and **Gunicorn** with **NGINX** as a reverse proxy. If you want to deploy a similar setup, follow these steps:

1. **Set up an EC2 instance**
2. **Install Python, Pip, and Virtual Environment**
3. **Clone this repository**
4. **Install dependencies**
5. **Set up PostgreSQL/MySQL**
6. **Configure Gunicorn and Nginx**
7. **Enable HTTPS (Optional)**

## Contributions
Feel free to fork this repository and submit a pull request if you want to contribute or improve the project.

## License
This project is licensed under the **MIT License**.

---

📌 **Maintainer:** Vikas Bansode  
📧 **Email:** vikasbansode804@gmail.com


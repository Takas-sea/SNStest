# SNStest Backend

## Overview
The core objective is to design and build a production-ready backend and cloud infrastructure, focusing on scalability, clean architecture, and clear DevOps practices rather than UI complexity.

## Tech Stack
- **FastAPI** (Python)
- **PostgreSQL**
- **Docker**
- **AWS ECS (Fargate)**
- **AWS RDS**
- **AWS ECR**
- **Terraform**
- **GitHub Actions (CI/CD)**

## Current Status 
- Project structure initialized  
- Basic directories created (`backend`, `infra`, `docs`)  
- API specifications drafted  
- ER diagram prepared  
- Architecture diagram prepared  

## API Specification (Draft)
These API endpoints represent the minimum features required for an SNS MVP.

### User
- `POST /users` — Create a new user  
- `POST /login` — User login (JWT planned)

### Posts
- `GET /posts` — Retrieve all posts  
- `POST /posts` — Create a new post  
- `GET /posts/{id}` — Retrieve a specific post  

Authentication, image uploads, and advanced features are intentionally excluded from the MVP scope.

## Directory Structure (Backend)
```
backend/
├── app/
│ └── init.py
├── Dockerfile
├── requirements.txt
└── README.md
```
## Notes
This backend focuses on reliability, clarity, and cloud deployment readiness rather than feature-rich functions.  
The primary evaluation points for this project are:
- Architectural planning  
- Infrastructure-as-Code skills  
- Cloud-native deployment  
- Clean API design  

Further enhancements will be made in subsequent days following the development plan.
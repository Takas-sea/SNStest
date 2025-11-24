# SNStest Infrastructure
## Overview
This directory contains the Infrastructure-as-Code (IaC) configuration for the SNStest application.
All AWS resources will be provisioned using **Terraform**, enabling reproducible, scalable, and maintainable cloud infrastructure.

The infrastructure is designed to support a production-ready deployment using a fully managed, container-based architecture.

---

## Architecture Components

### **1. Network Layer**
- **VPC** with public and private subnets
- **Internet Gateway / NAT Gateway** (planned)
- **Security Groups** with least-privilege configuration

### **2. Compute Layer**
- **Amazon ECS (Fargate)**
  - Serverless container orchestration
  - Scalable and managed runtime for the backend API

### **3. Load Balancing**
- **Application Load Balancer (ALB)**
  - Handles incoming HTTP requests
  - Health checks for ECS tasks

### **4. Storage / Database**
- **Amazon RDS (PostgreSQL)**
  - Managed relational database
  - Private subnet deployment for security

### **5. Container Registry**
- **Amazon ECR**
  - Stores container images built from GitHub Actions

### **6. CI/CD Pipeline**
- **GitHub Actions**
  - Builds Docker images
  - Pushes to ECR
  - Updates ECS task definitions
  - Triggers a zero-downtime deployment

---

## Directory Structure (Terraform)
```
infra/
├── main.tf # Entry point for Terraform resources
├── variables.tf # (Planned) Variables for configuration
├── outputs.tf # (Planned) Exported values
└── README.md
```

---

## Philosophy
The infrastructure focuses on:
- Reliability
- Security
- Scalability
- Clear and maintainable IaC
- Cloud-native best practices

This project demonstrates practical cloud engineering competence suitable for professional development and real-world deployment.

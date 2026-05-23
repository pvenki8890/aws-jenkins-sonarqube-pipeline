# AWS Jenkins DevSecOps CI/CD Pipeline

A complete end-to-end DevSecOps CI/CD pipeline built using Jenkins, Docker, SonarQube, Maven, Trivy, and AWS EC2 to automate application build, code quality analysis, vulnerability scanning, containerization, and deployment workflows.

---

## 🚀 Project Overview

This repository showcases a hands-on implementation of a production-style CI/CD pipeline designed with DevSecOps best practices. The pipeline automates the software delivery lifecycle while ensuring code quality, security validation, and deployment readiness.

The infrastructure and tooling were provisioned on an AWS EC2 instance and integrated together using Jenkins Pipeline as Code.

### ✨ Key Features

* Automated CI/CD Pipeline using Jenkins
* Static Code Analysis with SonarQube
* Docker Image Build & Containerization
* Vulnerability Scanning using Trivy
* Maven Build Automation
* Jenkins Shared Library Integration
* DockerHub Credential Management
* SonarQube Quality Gate Validation
* Webhook-based Tool Integration
* End-to-End DevSecOps Workflow

---

## 🛠️ Tech Stack & Tools

### Cloud & Infrastructure

* Amazon Web Services (AWS EC2)
* Ubuntu Linux

### DevOps & CI/CD

* Jenkins
* Jenkins Shared Libraries
* Git & GitHub

### Build & Quality Tools

* Maven
* SonarQube

### Security & Containerization

* Docker
* Trivy

---

## 📐 CI/CD Workflow Architecture

```text
Developer Commit
        ↓
GitHub Repository
        ↓
Jenkins Pipeline Trigger
        ↓
Source Code Checkout
        ↓
Maven Build & Packaging
        ↓
SonarQube Static Analysis
        ↓
Quality Gate Validation
        ↓
Docker Image Build
        ↓
Trivy Vulnerability Scan
        ↓
DockerHub Push
        ↓
Pipeline Cleanup & Reporting
```

---

## 🔄 Pipeline Stages

### 1️⃣ Source Code Checkout

Jenkins pulls the latest application code from GitHub SCM.

### 2️⃣ Build & Package

Maven compiles and packages the Java application.

### 3️⃣ Static Code Analysis

SonarQube scans the source code for:

* Bugs
* Vulnerabilities
* Code Smells
* Security Issues
* Maintainability Metrics

### 4️⃣ Quality Gate Validation

Pipeline waits for SonarQube Quality Gate approval before proceeding.

### 5️⃣ Docker Image Build

Application is containerized using Docker.

### 6️⃣ Vulnerability Scanning

Trivy scans the Docker image for:

* Critical Vulnerabilities
* High Severity CVEs
* Misconfigurations

### 7️⃣ DockerHub Push

Validated Docker image is pushed securely to DockerHub.

---

## 🔧 Jenkins Integrations

### SonarQube Integration

* SonarQube Server Configuration
* Sonar Token Authentication
* Webhook Integration
* Quality Gate Enforcement

### DockerHub Integration

* Secure Credentials Management
* Automated Docker Authentication

### Shared Library Integration

Reusable Jenkins pipeline code implemented using Jenkins Shared Libraries.

---

## 📊 Validation & Results

After successful pipeline execution, the following validations were performed:

* ✅ Jenkins Console Output Verification
* ✅ SonarQube Dashboard Quality Reports
* ✅ Trivy Vulnerability Reports
* ✅ Docker Image Build Verification
* ✅ DockerHub Push Validation

---

## 📷 Screenshots

### Jenkins Pipeline Execution

*Add your Jenkins pipeline screenshot here*

### SonarQube Dashboard

*Add your SonarQube quality gate screenshot here*

### Trivy Scan Results

*Add your Trivy vulnerability scan screenshot here*

---

## 🎯 Learning Outcomes

Through this project, I gained practical experience in:

* CI/CD Pipeline Automation
* DevSecOps Best Practices
* Jenkins Pipeline as Code
* Docker Containerization
* Static Code Analysis
* Security Scanning Automation
* AWS Infrastructure Setup
* Credential & Secret Management
* Tool Integration & Automation

---

## 📌 Future Improvements

* Kubernetes Deployment Integration
* Terraform Infrastructure Automation
* Helm Chart Deployment
* Multi-Environment Pipelines
* Automated Deployment Strategies
* Slack/Email Notifications
* Artifact Management using JFrog

---

## 🤝 Contributing

Contributions and suggestions are welcome.

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to your branch
5. Create a Pull Request

---

## 📄 Reference

This project was implemented as part of a hands-on DevOps and CI/CD exercise using Jenkins, SonarQube, Docker, Maven, Trivy, and AWS services.

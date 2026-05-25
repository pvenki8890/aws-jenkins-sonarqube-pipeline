# 🚀 AWS Jenkins DevSecOps CI/CD Pipeline

A production-style end-to-end DevSecOps CI/CD pipeline built using Jenkins, Maven, SonarQube, Docker, Trivy, and AWS EC2. This project automates the software delivery lifecycle including build, testing, code quality analysis, containerization, vulnerability scanning, and Docker image publishing.

---

# 📌 Project Overview

This project demonstrates a complete hands-on implementation of a modern DevSecOps CI/CD workflow using Jenkins Pipeline as Code.

The pipeline was built and configured on an AWS EC2 Ubuntu server and integrates multiple DevOps tools to automate continuous integration and delivery processes for a Java Spring Boot application.

The objective of this project was to gain real-world hands-on experience with:

- CI/CD Pipeline Automation
- DevSecOps Tool Integration
- Docker Containerization
- Jenkins Shared Libraries
- Maven Build Lifecycle
- AWS Infrastructure Setup
- Troubleshooting & Pipeline Debugging

---

# 🛠️ Tech Stack

## ☁️ Cloud & Infrastructure

- Amazon EC2
- Ubuntu Linux

## ⚙️ CI/CD & DevOps

- Jenkins
- Jenkins Shared Libraries
- Git
- GitHub

## 🧪 Build & Quality Tools

- Maven
- SonarQube

## 🔐 Security & Containerization

- Docker
- Trivy

---

# 📐 CI/CD Workflow Architecture

```text
Developer Commit
        ↓
GitHub Repository
        ↓
Jenkins Pipeline Trigger
        ↓
Git Checkout
        ↓
Maven Unit Testing
        ↓
Integration Testing
        ↓
SonarQube Static Code Analysis
        ↓
Maven Build & Packaging
        ↓
Docker Image Build
        ↓
Trivy Security Scan
        ↓
DockerHub Push
        ↓
Cleanup & Reporting
🔄 Pipeline Stages
1️⃣ Git Checkout

Jenkins pulls the latest source code from the GitHub repository.

2️⃣ Unit Testing

Maven executes automated unit tests to validate application functionality.

Tools Used
Maven
JUnit
3️⃣ Integration Testing

Integration tests are executed as part of the CI workflow.

4️⃣ Static Code Analysis - SonarQube

SonarQube performs code quality and security analysis.

Validations Performed
Bugs Detection
Vulnerabilities
Code Smells
Maintainability Analysis
Security Hotspots
5️⃣ Maven Build & Packaging

Application is packaged into an executable JAR file using Maven.

6️⃣ Docker Image Build

The Spring Boot application is containerized using Docker.

Docker Features
Lightweight container image
Portable deployment
Consistent runtime environment
7️⃣ Trivy Vulnerability Scanning

Trivy scans the Docker image for:

Critical Vulnerabilities
High Severity CVEs
Misconfigurations
8️⃣ DockerHub Push

Successfully validated Docker images are pushed securely to DockerHub.

9️⃣ Docker Cleanup

Local Docker images and temporary resources are cleaned up after execution.

🔧 Jenkins Integrations
✅ SonarQube Integration
SonarQube Server Configuration
Authentication using Access Tokens
Jenkins-SonarQube Integration
Quality Gate Validation
✅ DockerHub Integration
Secure DockerHub Credentials
Automated Docker Login
Image Push Automation
✅ Shared Library Integration

Reusable Jenkins pipeline functions implemented using Jenkins Shared Libraries for modular and maintainable pipeline code.

📊 Project Validation

The following validations were successfully completed:

✅ Maven Build Success
✅ Unit Test Execution
✅ Integration Test Execution
✅ Docker Image Build
✅ DockerHub Push
✅ Jenkins Pipeline Automation
✅ Shared Library Integration
✅ SonarQube Integration
✅ End-to-End CI/CD Workflow
📷 Screenshots
Jenkins Successful Pipeline
<img width="1900" height="902" alt="Jenkins stage view" src="https://github.com/user-attachments/assets/ff1c6593-2ee7-4791-b6d2-5bb4a797f600" />

Console Output final Success
<img width="793" height="1027" alt="Console Output final Success" src="https://github.com/user-attachments/assets/b7789f97-b008-4cfd-b39a-227b1e96d83d" />

DockerHub pushed image
<img width="1900" height="903" alt="DockerHub pushed image" src="https://github.com/user-attachments/assets/4aa21edc-8579-48f5-9162-088dc9114b12" />

EC2 Setup
<img width="1907" height="823" alt="EC2 setup1" src="https://github.com/user-attachments/assets/d9bd3f68-bfed-4cc1-9d51-b868854ca018" />

Jenkins stage view
<img width="1900" height="902" alt="Jenkins stage view" src="https://github.com/user-attachments/assets/9c6e28a2-4082-495d-a14c-5a1a9bba5398" />

GitHub repo
<img width="940" height="896" alt="GitHub repo2" src="https://github.com/user-attachments/assets/93bf9fe6-99ab-4757-b27d-d61b02fa15e8" />

⚠️ Infrastructure Notes

Due to EC2 infrastructure resource limitations during testing:

SonarQube Quality Gate stage was temporarily skipped
Trivy scan stage was temporarily disabled during final execution

These stages were successfully configured and tested independently during implementation.

🎯 Key Learning Outcomes

Through this project, I gained practical hands-on experience in:

CI/CD Pipeline Design
Jenkins Pipeline as Code
DevSecOps Best Practices
Docker Containerization
SonarQube Integration
Vulnerability Scanning
AWS EC2 Administration
Linux Troubleshooting
Jenkins Shared Libraries
Credential & Secret Management
Docker Permissions Management
Real-world Pipeline Debugging
🚀 Future Enhancements
Kubernetes Deployment Integration
Helm Chart Deployment
Terraform Infrastructure Automation
GitHub Webhook Automation
Multi-Environment Deployment Pipelines
Slack/Email Notifications
Artifact Management using JFrog
Production-grade Monitoring & Logging
🤝 Contributing

Contributions, suggestions, and improvements are welcome.

Steps to Contribute
Fork the repository
Create a feature branch
Commit your changes
Push to your branch
Open a Pull Request
📄 Conclusion

This project provided practical real-world exposure to designing and troubleshooting a complete DevSecOps CI/CD pipeline using industry-standard tools and AWS infrastructure.

It demonstrates hands-on implementation of:

Continuous Integration
Continuous Delivery
Security Scanning
Containerization
Infrastructure Automation
Jenkins Pipeline Orchestration










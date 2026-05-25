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

### 🔗 Repository Link
👉 https://github.com/pvenki8890/Java_app_3.0

---

# 📐 CI/CD Workflow Architecture

```text
┌──────────────────────┐
│  Developer Commit    │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│  GitHub Repository   │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ Jenkins Pipeline     │
│ Triggered            │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│  Git Checkout        │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│  Maven Unit Testing  │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ Integration Testing  │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ SonarQube Static     │
│ Code Analysis        │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ Maven Build &        │
│ Packaging            │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ Docker Image Build   │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ Trivy Security Scan  │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ DockerHub Push       │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ Cleanup & Reporting  │
└──────────────────────┘
```

---

# 🔄 Pipeline Stages

---

## 1️⃣ Git Checkout

Jenkins pulls the latest source code from the GitHub repository to ensure the pipeline always uses the most recent application changes.

### ✅ Purpose
- Fetch latest code from SCM
- Trigger automated CI workflow
- Maintain version-controlled builds

---

## 2️⃣ Maven Unit Testing

Maven executes automated unit tests to validate application functionality before moving further in the pipeline.

### 🛠️ Tools Used
- Maven
- JUnit

### ✅ Validations
- Application logic verification
- Test case execution
- Build integrity checks

---

## 3️⃣ Integration Testing

Integration tests validate communication between application modules and dependencies.

### ✅ Purpose
- Verify module integration
- Validate application workflow
- Prevent runtime conflicts

---

## 4️⃣ Static Code Analysis - SonarQube

SonarQube performs deep static code analysis to identify quality and security issues.

### 🔍 Validations Performed

- 🐛 Bug Detection
- 🔒 Vulnerability Analysis
- 🧄 Code Smell Detection
- 📈 Maintainability Analysis
- 🚨 Security Hotspots

---

## 5️⃣ Maven Build & Packaging

The Spring Boot application is compiled and packaged into an executable production-ready JAR file.

### ✅ Build Outputs
- Compiled Java Classes
- Packaged Spring Boot JAR
- Production Build Artifact

---

## 6️⃣ Docker Image Build

The application is containerized using Docker to provide consistent deployment environments.

### 🚀 Benefits
- Lightweight Containers
- Portable Deployments
- Environment Consistency
- Faster Application Delivery

---

## 7️⃣ Trivy Vulnerability Scanning

Trivy scans the generated Docker image to enforce DevSecOps security best practices.

### 🔐 Scan Coverage
- Critical Vulnerabilities
- High Severity CVEs
- OS Package Vulnerabilities
- Dependency Vulnerabilities
- Misconfigurations

---

## 8️⃣ DockerHub Push

Validated Docker images are securely pushed to DockerHub for deployment readiness.

### ✅ Features
- Automated Docker Login
- Secure Credential Management
- Image Versioning & Tagging

---

## 9️⃣ Docker Cleanup & Reporting

Temporary Docker images and build resources are cleaned from the Jenkins server after successful execution.

### ✅ Cleanup Activities
- Local Image Cleanup
- Workspace Optimization
- Build Reporting

---

# 🔧 Jenkins Integrations

---

## ✅ SonarQube Integration

Integrated SonarQube with Jenkins for automated code quality analysis and security validation.

### 🔹 Features
- SonarQube Server Configuration
- Token-based Authentication
- Jenkins-SonarQube Integration
- Automated Static Code Analysis
- Quality Gate Validation

---

## ✅ DockerHub Integration

DockerHub integration was configured for secure image publishing.

### 🔹 Features
- Secure Docker Credentials
- Automated Docker Authentication
- Docker Image Push Automation

---

## ✅ Shared Library Integration

Reusable Jenkins pipeline logic implemented using Jenkins Shared Libraries.

### 🔹 Benefits
- Modular Pipeline Code
- Reusable Functions
- Centralized Pipeline Management
- Cleaner Jenkinsfiles

---

# 📊 Project Validation

The following validations were successfully completed during project implementation:

- ✅ Maven Build Success
- ✅ Unit Test Execution
- ✅ Integration Test Execution
- ✅ Docker Image Build
- ✅ DockerHub Push
- ✅ Jenkins Pipeline Automation
- ✅ Shared Library Integration
- ✅ SonarQube Integration
- ✅ End-to-End CI/CD Workflow Validation

---

# 📷 Screenshots

---

## 🖥️ Jenkins Successful Pipeline

> Add Jenkins Stage View Screenshot

---

## 📄 Jenkins Console Output

> Add Final Successful Build Console Screenshot

---

## 🐳 DockerHub Repository

> Add DockerHub Pushed Image Screenshot

---

## ☁️ AWS EC2 Setup

> Add AWS EC2 Infrastructure Screenshot

---

## 📁 GitHub Repository

> Add GitHub Repository Screenshot

---

# ⚠️ Infrastructure Notes

Due to temporary EC2 infrastructure limitations during testing:

- SonarQube Quality Gate stage was temporarily skipped
- Trivy scan stage was temporarily disabled during final execution

Both stages were successfully configured and tested independently during implementation.

---

# 🎯 Key Learning Outcomes

Through this project, I gained practical hands-on experience in:

- CI/CD Pipeline Design
- Jenkins Pipeline as Code
- DevSecOps Best Practices
- Docker Containerization
- SonarQube Integration
- Vulnerability Scanning
- AWS EC2 Administration
- Linux Troubleshooting
- Jenkins Shared Libraries
- Credential & Secret Management
- Docker Permission Management
- Real-world Pipeline Debugging

---

# 🚀 Future Enhancements

- Kubernetes Deployment Integration
- Helm Chart Deployment
- Terraform Infrastructure Automation
- GitHub Webhook Automation
- Multi-Environment Pipelines
- Slack / Email Notifications
- Artifact Management using JFrog
- Production-grade Monitoring & Logging

---

# 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

## 📌 Steps to Contribute

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to your branch
5. Open a Pull Request

---

# 📄 Conclusion

This project provided practical real-world exposure to designing, implementing, and troubleshooting a complete DevSecOps CI/CD pipeline using industry-standard tools and AWS infrastructure.

### 🚀 Technologies & Concepts Demonstrated

- Continuous Integration
- Continuous Delivery
- DevSecOps Automation
- Security Scanning
- Docker Containerization
- Infrastructure Automation
- Jenkins Pipeline Orchestration
- Cloud-based CI/CD Workflows

---


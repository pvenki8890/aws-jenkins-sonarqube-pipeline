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

---

##🔄 Pipeline Stages
###1️⃣ Git Checkout
Jenkins pulls the latest source code from the GitHub repository to ensure the build uses the most recent updates.

###2️⃣ Unit Testing
Maven executes automated unit tests to validate application functionality before moving forward.

Tools Used: Maven, JUnit

###3️⃣ Integration Testing
Integration tests are executed as part of the CI workflow to ensure different modules work together seamlessly.

###4️⃣ Static Code Analysis (SonarQube)
SonarQube performs deep code quality and security analysis.

Validations Performed:

🐛 Bugs Detection

🔒 Vulnerabilities & Security Hotspots

🧄 Code Smells

📈 Maintainability Analysis

5️⃣ Maven Build & Packaging
The Spring Boot application is compiled and packaged into a production-ready, executable JAR file using Maven.

6️⃣ Docker Image Build
The application is containerized using Docker to ensure environment consistency.

Key Benefits: Lightweight container images, highly portable deployment, and consistent runtime environments.

7️⃣ Trivy Vulnerability Scanning
Trivy scans the generated Docker image to enforce DevSecOps security guardrails.

Scans For: Critical Vulnerabilities, High Severity CVEs, and OS/Package Misconfigurations.

8️⃣ DockerHub Push
Successfully validated and secure Docker images are pushed directly to DockerHub for deployment readiness.

9️⃣ Docker Cleanup & Reporting
Local Docker images and temporary build resources are scrubbed from the Jenkins agent to optimize storage, followed by final pipeline reporting.

🔧 Jenkins Integrations
✅ SonarQube Integration
• SonarQube Server Configuration
• Authentication using Access Tokens
• Jenkins-SonarQube Integration
• Quality Gate Validation
✅ DockerHub Integration
• Secure DockerHub Credentials
• Automated Docker Login
• Image Push Automation
✅ Shared Library Integration

Reusable Jenkins pipeline functions implemented using Jenkins Shared Libraries for modular and maintainable pipeline code.

📊 Project Validation

The following validations were successfully completed:

• ✅ Maven Build Success
• ✅ Unit Test Execution
• ✅ Integration Test Execution
• ✅ Docker Image Build
• ✅ DockerHub Push
• ✅ Jenkins Pipeline Automation
• ✅ Shared Library Integration
• ✅ SonarQube Integration
• ✅ End-to-End CI/CD Workflow
📷 Screenshots
Jenkins Successful Pipeline

Console Output final Success

DockerHub pushed image

EC2 Setup

Jenkins stage view


GitHub repo

⚠️ Infrastructure Notes

Due to EC2 infrastructure resource limitations during testing:

• SonarQube Quality Gate stage was temporarily skipped
• Trivy scan stage was temporarily disabled during final execution

These stages were successfully configured and tested independently during implementation.

🎯 Key Learning Outcomes

Through this project, I gained practical hands-on experience in:

• CI/CD Pipeline Design
• Jenkins Pipeline as Code
• DevSecOps Best Practices
• Docker Containerization
• SonarQube Integration
• Vulnerability Scanning
• AWS EC2 Administration
• Linux Troubleshooting
• Jenkins Shared Libraries
• Credential & Secret Management
• Docker Permissions Management
• Real-world Pipeline Debugging
🚀 Future Enhancements
• Kubernetes Deployment Integration
• Helm Chart Deployment
• Terraform Infrastructure Automation
• GitHub Webhook Automation
• Multi-Environment Deployment Pipelines
• Slack/Email Notifications
• Artifact Management using JFrog
• Production-grade Monitoring & Logging
🤝 Contributing

Contributions, suggestions, and improvements are welcome.

Steps to Contribute
1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to your branch
5. Open a Pull Request
📄 Conclusion

This project provided practical real-world exposure to designing and troubleshooting a complete DevSecOps CI/CD pipeline using industry-standard tools and AWS infrastructure.

It demonstrates hands-on implementation of:

• Continuous Integration
• Continuous Delivery
• Security Scanning
• Containerization
• Infrastructure Automation
• Jenkins Pipeline Orchestration










Project Overview

# CI/CD Pipeline with Jenkins, SonarQube, Docker & Trivy

This project demonstrates a complete CI/CD pipeline implementation using Jenkins integrated with SonarQube, Docker, Maven, and Trivy on AWS EC2.

Architecture Diagram:

Developer Push
      ↓
   GitHub
      ↓
   Jenkins
      ↓
 Maven Build
      ↓
 SonarQube Scan
      ↓
 Docker Build
      ↓
 Trivy Scan
      ↓
 DockerHub

** Tools Used:**
- AWS EC2
- Jenkins
- Docker
- Maven
- SonarQube
- Trivy
- GitHub

 **Learning Outcomes:**
- Learn Jenkins pipeline setup
- Integrated SonarQube with Jenkins
- Configured Docker builds
- Performed vulnerability scanning using Trivy
- Configured Jenkins Shared Libraries

**Credits Section:**
## Credits

Some installation scripts and learning references were adapted from:
https://github.com/praveen1994dec

This project was implemented for learning and hands-on practice purposes.


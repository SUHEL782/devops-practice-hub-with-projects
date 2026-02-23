This project demonstrates the end-to-end implementation of a complete CI/CD pipeline using modern DevOps tools and practices including Terraform, Ansible, Jenkins, SonarQube, JFrog, Docker, Kubernetes (EKS), Prometheus, and Grafana.

 Step-by-Step Implementation
🔹 1. Infrastructure Provisioning (Terraform)

Created:

VPC

Security Groups

Ansible Controller

Jenkins Master & Agent Nodes

Automated provisioning using Terraform

🔹 2. SSH Configuration

Configured passwordless SSH authentication

Enabled seamless communication between:

Ansible Controller

Jenkins Nodes

🔹 3. Jenkins Setup (via Ansible)

Installed & configured:

Jenkins Master

Jenkins Agent

Configured Agent as Maven Build Server

🔹 4. Jenkins Master-Agent Integration

Added Agent credentials in Jenkins Master

Established secure communication between nodes

🔹 5. GitHub Integration

Added GitHub credentials in Jenkins

Created Multibranch Pipeline Job

🔹 6. Webhook Automation

Configured GitHub Webhook Trigger

Used Multibranch Scan Webhook Plugin

Enabled automatic pipeline execution on code push

 7. SonarQube (Code Quality & Security)

Generated SonarCloud Token

Configured SonarQube in Jenkins

Installed required plugins

Added:

Code Analysis Stage

Unit Testing Stage

Build Stage

Created sonar-project.properties

 8. JFrog Artifactory Integration

Integrated Jenkins with JFrog Artifactory

Stored build artifacts securely

 9. Docker Build & Push

Built Docker image from .jar

Pushed image to JFrog Artifactory Docker Repo

Automated using Jenkins Pipeline

 10. Kubernetes (EKS Setup)

Provisioned EKS Cluster using Terraform

Installed:

kubectl

AWS CLI v2

Connected cluster using:

aws eks update-kubeconfig --region <region> --name <cluster>
11. Deployment on Kubernetes

Pulled Docker image from Artifactory

Created:

Deployment

Service (LoadBalancer)

Used Kubernetes Secrets for secure image pull

Deployed application in EKS

 12. Monitoring (Prometheus + Grafana)

Installed via Helm

Configured:

Prometheus for metrics

Grafana for visualization

Changed service type to LoadBalancer for external access

🎯 Key Highlights

✔ End-to-End CI/CD Automation
✔ Infrastructure as Code (Terraform)
✔ Configuration Management (Ansible)
✔ Code Quality (SonarQube)
✔ Artifact Management (JFrog)
✔ Containerization (Docker)
✔ Orchestration (Kubernetes - EKS)
✔ Monitoring (Prometheus + Grafana)

⭐ Support

If you found this project helpful for learning DevOps:

👉 Don’t forget to Star ⭐ the repository

🔗 Connect with Me

👨‍💻 Suhel Khan
 DevOps & Cloud Enthusiast

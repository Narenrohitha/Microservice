# 🛒 Cloud-Native E-Commerce Microservices DevSecOps Project

A production-grade **Online Shopping Microservices Application** built with modern DevSecOps practices using:


<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/720bb75c-555d-41d5-9cbc-35ed4f5d6cef" />



* Kubernetes (EKS)
* Docker
* Jenkins CI/CD
* SonarQube
* Trivy
* GitOps (Argo CD)
* Prometheus & Grafana Monitoring
* AWS Load Balancer Controller

This project is a customized and extended implementation of the Google Cloud Platform microservices demo, enhanced with a complete DevSecOps production pipeline and AWS EKS deployment.

🔗 GitHub Repository:
[https://github.com/Narenrohitha/Microservice](https://github.com/Narenrohitha/Microservice)

---

# 🚀 Project Overview

Online Boutique is a cloud-native microservices-based e-commerce application where users can:

* Browse products
* Add items to cart
* Checkout securely
* Receive order confirmation
* View recommendations

This implementation demonstrates:

✔ CI/CD automation
✔ Container security scanning
✔ Static code analysis
✔ Kubernetes production deployment
✔ GitOps workflow
✔ Monitoring & Observability
✔ Cloud Load Balancing

---

# 🏗️ Architecture Overview

This application consists of 11 independent microservices:

| Service               | Language        | Description                         |
| --------------------- | --------------- | ----------------------------------- |
| frontend              | Go              | Serves web UI and manages sessions  |
| productcatalogservice | Go              | Provides product listing and search |
| shippingservice       | Go              | Calculates shipping cost (mock)     |
| checkoutservice       | Go              | Orchestrates order workflow         |
| cartservice           | C#              | Stores cart items in Redis          |
| currencyservice       | Node.js         | Handles currency conversion         |
| paymentservice        | Node.js         | Processes payments (mock)           |
| emailservice          | Python          | Sends order confirmation            |
| recommendationservice | Python          | Recommends products                 |
| loadgenerator         | Python (Locust) | Simulates user traffic              |
| adservice             | Java            | Provides contextual ads             |

---

# 🧱 Technology Stack

### 🔹 Backend

* Go
* Node.js
* Python
* C#
* Java

### 🔹 DevOps & CI/CD

* Jenkins
* Docker
* DockerHub (narenganeshan)
* SonarQube
* OWASP Dependency Check
* Trivy

### 🔹 Kubernetes & Cloud

* Amazon EKS
* AWS CLI
* kubectl
* eksctl
* Helm
* AWS Load Balancer Controller

### 🔹 GitOps

* Argo CD

### 🔹 Monitoring

* Prometheus
* Grafana
* Node Exporter

---

# ⚙️ DevSecOps Pipeline Flow

1. Developer pushes code to GitHub
2. Jenkins pipeline triggers automatically
3. Code quality scan using SonarQube
4. Dependency scanning using OWASP
5. Container vulnerability scan using Trivy
6. Docker image built and pushed to DockerHub
7. Argo CD deploys updated image to EKS
8. Prometheus & Grafana monitor cluster

---

# 🖥️ Infrastructure Requirements

* Instance Type: c5.xlarge (recommended)
* Ubuntu/Debian OS
* Open Ports:

  * 22 (SSH)
  * 80 (HTTP)
  * 443 (HTTPS)
  * 8080 (Jenkins)
  * 9000 (SonarQube)

---

# 🛠️ Tools Installed

* OpenJDK 17 / 21
* Jenkins
* Docker Engine
* Trivy
* AWS CLI
* kubectl
* eksctl
* Helm
* SonarQube (Docker Container)

---

# ☁️ AWS EKS Setup Highlights

* EKS Cluster creation via eksctl
* Managed Nodegroup configuration
* IAM OIDC association
* AWS Load Balancer Controller installation
* Ingress setup via ALB
* Secure Service Account configuration

---

# 📊 Monitoring Stack

Installed using Helm:

* kube-prometheus-stack
* Prometheus
* Grafana
* Node Exporter

### Grafana Default Credentials:

* Username: admin
* Password: prom-operator

Dashboards:

* Kubernetes Monitoring
* Node Exporter
* Namespace Monitoring

---

# 🔁 GitOps Deployment (Argo CD)

* Argo CD installed via Helm
* LoadBalancer exposure configured
* Automated synchronization from GitHub
* Production-style GitOps workflow

---

# 🔐 Security Practices Implemented

* Static Code Analysis (SonarQube)
* Dependency Vulnerability Scan (OWASP)
* Container Image Scan (Trivy)
* IAM Role-based access
* Kubernetes RBAC
* Secure SMTP configuration
* DockerHub credential management

---

# 🧹 Cleanup (Cluster Deletion)


---

# 📌 Notes

* Replace placeholders like `<your-server-ip>` before deployment.
* Always pin versions in production environments.
* Follow official documentation for updates.
* Apache-2.0 license retained from original source.



# 🎯 What This Project Demonstrates

This project showcases:

* Real-world DevSecOps implementation
* Kubernetes production deployment
* CI/CD automation
* Secure container practices
* GitOps-based release management
* Cloud-native architecture

This project is strong — now your branding matches the quality.

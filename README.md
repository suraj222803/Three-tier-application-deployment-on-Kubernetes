# Three-Tier Application Deployment on Kubernetes (EKS)

This repository contains a complete implementation of a **Three-Tier Application** deployed on **Kubernetes (Amazon EKS)**.  
The application is containerized using Docker and orchestrated using Kubernetes services and ingress.

---

## 🏗️ Architecture

The application follows a three-tier architecture:

1. **Frontend**
   - React-based UI
   - Exposed to users via Kubernetes Ingress

2. **Backend**
   - Node.js / Express REST API
   - Communicates with MongoDB

3. **Database**
   - MongoDB
   - Deployed inside the Kubernetes cluster

---

## 🛠️ Tech Stack

- AWS (EKS, ECR, IAM)
- Docker
- Kubernetes
- kubectl
- eksctl
- Helm
- AWS Load Balancer Controller

---

## 📁 Project Structure

```text
.
├── frontend/
│   ├── Dockerfile
│   └── source code
├── backend/
│   ├── Dockerfile
│   └── source code
├── k8s_manifests/
│   ├── frontend-deployment.yaml
│   ├── frontend-service.yaml
│   ├── backend-deployment.yaml
│   ├── backend-service.yaml
│   ├── full_stack_lb.yaml
│   └── mongo/
│       ├── mongo-deployment.yaml
│       └── mongo-service.yaml
└── README.md


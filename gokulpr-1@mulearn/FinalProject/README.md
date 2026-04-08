# My First Scalable Web App - Final Project

## 📋 Project Overview

This is the final project for Shipyard Foundations, demonstrating a complete workflow of:
- Creating a simple web application
- Packaging it with Docker
- Deploying it to Kubernetes with multiple replicas
- Testing self-healing capabilities

## 📁 Files Included

- **index.html** - Professional portfolio-style web application
- **Dockerfile** - Container definition using nginx:alpine
- **deployment.yaml** - Kubernetes deployment with 3 replicas

## 🚀 Setup & Deployment

### Prerequisites
- Docker installed
- Kind (Kubernetes in Docker) installed
- kubectl installed

### Step 1: Build Docker Image
```bash
docker build -t scalable-web-app:latest .
```

### Step 2: Start KIND Cluster
```bash
kind create cluster --name shipyard
```

### Step 3: Load Docker Image to KIND
```bash
kind load docker-image scalable-web-app:latest --name shipyard
```

### Step 4: Deploy to Kubernetes
```bash
kubectl apply -f deployment.yaml
```

### Step 5: Verify Deployment
```bash
kubectl get deployments
kubectl get pods
kubectl logs -f deployment/scalable-web-app
```

### Step 6: Access the Application
```bash
kubectl port-forward service/scalable-web-app 8080:80
```
Then open http://localhost:8080 in your browser.

## 🛡️ Self-Healing Test

Test the self-healing capability by deleting a pod:

```bash
# List all pods
kubectl get pods

# Delete a specific pod
kubectl delete pod <pod-name>

# Verify a new pod is created automatically
kubectl get pods
```

## 📊 Features

✅ Containerized application with Docker
✅ Multi-replica Kubernetes deployment
✅ Environment variable configuration (STUDENT_NAME)
✅ Self-healing with automatic pod recreation
✅ Resource limits and requests
✅ Production-ready nginx configuration

## 🎓 Learning Outcomes

- Docker containerization basics
- Kubernetes deployment management
- Replica scaling concepts
- Pod self-healing demonstration
- Container orchestration workflow

## 📤 Submission Details

- **Student Name:** GOKUL P R
- **Project Path:** gokulpr-1@mulearn/FinalProject/
- **Tags:** #evn-dop-shipyard26-ship

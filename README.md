# 🚀 My First Kubernetes Project

A beginner-friendly Kubernetes project that demonstrates how to deploy a simple HTML website using Docker and Kubernetes.

---

## 📌 Project Overview

In this project, I:

* Created a simple HTML website
* Containerized the application using Docker
* Pushed the Docker image to Docker Hub
* Deployed the application on Kubernetes using Minikube
* Exposed the application using a Kubernetes Service
* Uploaded the complete project to GitHub

---

## 🛠️ Technologies Used

* HTML
* Docker
* Kubernetes
* Minikube
* Kubectl
* GitHub

---

## 📂 Project Structure

```text
my-project
│
├── index.html
├── Dockerfile
├── deployment.yaml
├── service.yaml
└── README.md
```

---

## Build Docker Image

```bash
docker build -t mywebsite:v1 .
```

Run Container:

```bash
docker run -d -p 8080:80 mywebsite:v1
```

---

## Push Image to Docker Hub

```bash
docker login
docker tag mywebsite:v1 your-dockerhub-username/mywebsite:v1
docker push your-dockerhub-username/mywebsite:v1
```

---

## Start Kubernetes

```bash
minikube start
```

Check cluster:

```bash
kubectl get nodes
```

---

## Deploy Application

```bash
kubectl apply -f deployment.yaml
```

Verify Pods:

```bash
kubectl get pods
```

---

## Create Service

```bash
kubectl apply -f service.yaml
```

Verify Service:

```bash
kubectl get svc
```

---

## Access Application

```bash
minikube service mywebsite-service --url
```

Open the generated URL in your browser.

---

## Kubernetes Workflow

```text
Developer
    │
    ▼
kubectl apply
    │
    ▼
Deployment
    │
    ▼
Pods
    │
    ▼
Service
    │
    ▼
Users
```

---

## Learning Outcomes

✅ Docker Image Creation

✅ Docker Hub Integration

✅ Kubernetes Deployments

✅ Kubernetes Services

✅ Pod Management

✅ Minikube Usage

✅ GitHub Project Management

---

## Future Improvements

* Deploy on AWS EC2
* Add Ingress Controller
* Configure CI/CD Pipeline
* Use Helm Charts
* Deploy on a Cloud Kubernetes Cluster

---

## Author

**Rahil Shaikh**

DevOps & Cloud Enthusiast 🚀

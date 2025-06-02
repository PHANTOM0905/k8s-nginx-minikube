# 🚀 Kubernetes NGINX Deployment on Minikube

This repository contains YAML configuration files to deploy a simple NGINX web server using Kubernetes locally on Minikube.

---

## 📦 Project Structure

- `deployment.yaml` – Defines the NGINX deployment with 2 replicas.
- `service.yaml` – Exposes the deployment using a NodePort service.

---

## 🎯 Objective

To deploy and manage containerized applications using Kubernetes on a local Minikube cluster as part of a DevOps internship task.

---

## 🛠️ Tools Used

- Kubernetes
- Minikube
- kubectl
- Docker

---

## 📂 Steps to Deploy

1. **Start Minikube**:
   ```bash
   minikube start
2. **Apply the deployment**:
    ```bash
    kubectl apply -f deployment.yaml
3. **Apply the service**:
    ```bash
    kubectl apply -f service.yaml
4. **Access the application**:
    ```bash
    minikube service nginx-service
5. **View pods**:
    ```bash
    kubectl get pods
6. **Scale deployements**:
    ```bash
    kubectl scale deployment nginx-deployment --replicas=3
7. **View logs**:
    ```bash
    kubectl describe pod <pod-name>

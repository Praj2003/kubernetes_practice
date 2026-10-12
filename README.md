
<img width="1640" height="494" alt="Kubernetes_Practice" src="https://github.com/user-attachments/assets/b01de850-dd44-4642-afb3-09bd4bef8f8b" />

## Overview
A beginner-friendly Kubernetes project implemented using **Minikube running inside Docker on AWS EC2** to understand Kubernetes fundamentals and service communication.

## Architecture
- **MongoDB:** Database deployed using a Kubernetes Deployment.
- **Mongo Express:** Web-based UI to interact with MongoDB.
- **Pods:** Run the MongoDB and Mongo Express containers.
- **NodePort Service:** Enables external access to Mongo Express.
- **ClusterIP Service:** Enables internal communication with MongoDB.
- **ConfigMap:** Stores non-sensitive configuration.
- **Secret:** Stores sensitive credentials.

## Technologies Used
- AWS EC2
- Docker
- Minikube
- Kubernetes
- MongoDB
- Mongo Express
- YAML

## Application Flow
1. Access Mongo Express through the NodePort Service.
2. Mongo Express connects to MongoDB using its ClusterIP Service.
3. Kubernetes Services route traffic to the appropriate Pods.
4. ConfigMaps and Secrets provide application configuration and credentials.

## Key Learnings
- Kubernetes Deployments and Pods
- Service discovery and networking
- NodePort vs. ClusterIP
- ConfigMaps and Secrets
- Running Minikube on cloud infrastructure

## Purpose
This project helped me build a practical understanding of Kubernetes resources, container orchestration, and communication between application components.

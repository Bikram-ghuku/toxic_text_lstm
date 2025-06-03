# Kubernetes Learning Project 🚀

This repository is a personal sandbox designed to learn and experiment with **Kubernetes** using **Minikube**. It includes a basic full-stack web application and deployment configuration files to understand how Kubernetes works in a local development environment.

## 📁 Repository Structure

```
.
├── backend/              # Node.js backend server (likely with Express.js)
├── frontend-reddit/      # Frontend client app (possibly built with React)
├── kubernetes/           # Kubernetes manifests (Deployments, Services, etc.)
└── .gitignore
```

## 🎯 Goals of the Project

- Learn the basics of Kubernetes architecture (Pods, Deployments, Services, etc.)
- Use **Minikube** to create a local Kubernetes cluster
- Containerize both frontend and backend apps with Docker
- Deploy the full-stack application on Kubernetes
- Explore service communication, scaling, and health checks

## 🛠️ Technologies Used

- **Frontend**: React (assumed from `frontend-reddit`)
- **Backend**: Node.js / Express.js (assumed from structure)
- **Containerization**: Docker
- **Kubernetes**: Minikube for local deployment

## 🚀 Getting Started

> Make sure you have Docker and Minikube installed on your system.

1. **Start Minikube**:

   ```bash
   minikube start
   ```

2. **Build Docker images inside Minikube**:

   ```bash
   eval $(minikube docker-env)
   docker build -t backend-image ./backend
   docker build -t frontend-image ./frontend-reddit
   ```

3. **Apply Kubernetes manifests**:

   ```bash
   kubectl apply -f kubernetes/
   ```

4. **Access the services**:

   ```bash
   minikube service frontend-service
   ```

   > Replace `frontend-service` with your actual service name defined in the YAML file.

## 📚 Learnings and Experiments

- Kubernetes deployment workflows
- Understanding `Deployment`, `Service`, and `Pod` lifecycle
- Using NodePort and ClusterIP services
- Connecting frontend to backend using Kubernetes DNS
- Scaling and updating services with `kubectl`

## 📦 Future Plans

- Add Ingress support
- Set up ConfigMaps and Secrets
- Implement CI/CD pipeline for auto-deployment

## 🙌 Acknowledgments

Built for self-learning and experimentation. Inspired by the need to deeply understand how to deploy and manage containerized apps at scale.

---

> This project is **not intended for production use**. It is purely for educational purposes.

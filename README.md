# Real Estate App - Kubernetes Manifests

## Overview
This repository contains **Kubernetes manifests** for deploying the Real Estate App on a **K3s cluster hosted on AWS.** 

Make sure you have completed [step 2](https://github.com/y7ksh-r/Real-estate-app-infra) before proceeding further.

## Features
- **Declarative Configuration**: All K8s resources are managed via YAML files.
- **Load Balancing**: Uses a Kubernetes **Ingress Controller**.
- **Auto-Healing & Scaling**: Ensures high availability.
- **Monitoring with Prometheus & Grafana**.

## Real-World Use Case
Deploying via Kubernetes allows the app to **scale efficiently**, handle high traffic loads, and maintain **zero-downtime deployments.**

## Deployment Steps
1. Clone the repository:
   ```sh
   git clone https://github.com/y7ksh-r/Real-estate-app.git
   cd real-estate-app/real-estate-k8s
   ```
2. Deploy the application:
   ```sh
   kubectl apply -f deployment.yaml
   ```
3. Verify pod status:
   ```sh
   kubectl get pods
   ```
4. Access the application via the **LoadBalancer or Ingress Controller**.

## Future Enhancements
- Integrate **ArgoCD for GitOps-based deployments**.
- Implement **service mesh (Istio or Linkerd) for better traffic control.**

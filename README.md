# Shamil's DevOps Pipeline Project

A small Flask app demonstrating a complete local CI/CD and deployment pipeline.

## What this project shows
- Dockerized a Python Flask application
- Built a CI/CD pipeline using GitHub Actions that automatically builds and pushes
  the Docker image to Docker Hub on every push to `main`
- Deployed the containerized app to a local Kubernetes cluster (Minikube) with
  a Deployment (2 replicas) and a NodePort Service

## Tools used
Docker, GitHub Actions, Docker Hub, Kubernetes (Minikube), Python/Flask

## How to run it yourself
1. Clone this repo
2. `docker build -t shamil-devops-app .`
3. `docker run -p 5000:5000 shamil-devops-app`
4. Or deploy to Kubernetes: `kubectl apply -f deployment.yaml -f service.yaml`
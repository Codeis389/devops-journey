# Complete DevOps Project - DevOps Blog

## Project Overview

- Build a professional blog with HTML/CSS
- Dockerized the application
- Set up CI/CD with GitHub Actions
- Deployed on Kubernets
- Monitored with Prometheus + Grafana

## Live URLs

- GitHub Pages: https://codeis389.github.io/devops-blog/
- GitHub Repo: https://github.com/Codeis389/devops-blog

## Tech Stack Used

- HTML/CSS - Frontend
- Docker - containerization
- GitHub Actions - CI/CD pipeline
- Kubernetes - container orchestration
- Prometheus - metrics collection
- Grafana - monitoring dashboard
- Nginx - web server inside container

## Key Commands Used

- docker build -t devops-blog .
- kubectl apply -f blog-deployment.yaml
- kubectl get pods
- minikube service devops-blog --url
- minikube service grafana -n monitoring --url

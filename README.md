# Mini DevOps Project

A small static website used to practise an end-to-end DevOps deployment workflow.

## Technology
- HTML and CSS
- Docker with Nginx
- Docker Hub
- Kubernetes (K3s)
- Terraform
- GitHub Actions
- AWS EC2

## Run locally without Docker

Open `index.html` in a browser.

## Build and run with Docker

```bash
docker build -t mini-devops-web:v1 .
docker run --name mini-devops-web -d -p 8080:80 mini-devops-web:v1
```

Open http://localhost:8080

To stop and remove the container:

```bash
docker rm -f mini-devops-web
```

## Project learning path

1. Commit the source code to GitHub.
2. Build and test the Docker image locally.
3. Push the image to Docker Hub.
4. Provision a small AWS EC2 instance with Terraform.
5. Install K3s and deploy the image to Kubernetes.
6. Automate image build and deployment with GitHub Actions.

## Note

This repository starts with the application and Dockerfile. Terraform, Kubernetes manifests, and CI/CD workflow files will be added during the corresponding learning phases.

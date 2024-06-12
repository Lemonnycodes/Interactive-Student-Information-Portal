# Student Information Portal - Full Stack Application [Part 2]


## Overview

This project focuses on containerization of web application, deployment on Kubernetes, and setting up a CI/CD pipeline. Web app has now been enhanced to ensure scalability and resiliency.

## Features

- **Containerization**: The application is containerized using Docker.
- **Kubernetes Deployment**: The application is deployed on Kubernetes with at least three pods running continuously.
- **CI/CD Pipeline**: Automated build and deployment are managed using Jenkins and GitHub.

## Project Structure

- **src/**: Contains the source code of the web application.
- **Dockerfile**: Defines the Docker image for the application.
- **Jenkinsfile**: Jenkins pipeline configuration for CI/CD.
- **k8s/**: Contains Kubernetes deployment YAML files.

## Getting Started

### Prerequisites

- Docker
- Kubernetes (Minikube, Rancher, EKS, or GKE)
- Jenkins
- Git

### Installation

1. **Clone the repository**
   ```bash
   clone the repository
   cd trial
   ```

2. **Build Docker Image**
   ```bash
   docker build -t your-dockerhub-username/ContainerizedAppDeployment-app .
   ```

3. **Push Docker Image to DockerHub**
   ```bash
   docker push your-dockerhub-username/ContainerizedAppDeployment-app
   ```

4. **Deploy on Kubernetes**
   - **Using kubectl**
     ```bash
     kubectl apply -f k8s/deployment.yaml
     kubectl apply -f k8s/service.yaml
     ```

   - **Using Rancher**
     Follow the Rancher documentation to set up and deploy the application: [Rancher Documentation](https://rancher.com/docs)

5. **Set up Jenkins for CI/CD**
   - Install Jenkins following the official [Jenkins Installation Guide](https://www.jenkins.io/doc/book/installing/)
   - Configure Jenkins with the provided Jenkinsfile.

## Tools and Technologies Used

- **Docker**: Containerization platform.
- **Kubernetes**: Container orchestration platform.
- **Jenkins**: Automation server for CI/CD.
- **GitHub**: Source code repository.

## SKILLS AQUIRED

- **Containerization**: Learned how to create Docker images and manage containers.
- **Kubernetes**: Gained experience in deploying and managing applications on Kubernetes.
- **CI/CD**: Understood the importance of automated build and deployment pipelines.

## PART 1 : https://github.com/Lemonnycodes/Student-Information-Portal-



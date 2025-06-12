![Architecture Diagram](https://github.com/LondheShubham153/reddit-clone-k8s-ingress/assets/71492927/e1eec5f2-1983-445b-8966-e9acfdea7f8e)






# Reddit Clone App on Kubernetes
This project demonstrates how to deploy a Reddit clone app on Kubernetes and expose it to the world using Minikube as the cluster.
Below is an overview of the architecture of this Reddit Clone App running on Kubernetes.

## Prerequisites
Before you begin, you should have the following tools installed on your local machine: 

- Docker
- Minikube cluster ( Running )
- kubectl
- Git

## Installation
Follow these steps to install and run the Reddit clone app on your local machine:

1) Clone this repository to your local machine: `git clone https://github.com/TusharGadhave/Reddit-clone-k8s`
2) Navigate to the project directory: `cd Reddit-clone-k8s`
3) Build the Docker image for the Reddit clone app: `docker build -t reddit-clone-app .`
4) Deploy the app to Kubernetes: `kubectl apply -f deployment.yaml`
5) Deploy the Service for deployment to Kubernetes: `kubectl apply -f service.yaml`
6) Expose the app as a Kubernetes service: `kubectl expose deployment reddit-deployment --type=NodePort --port=5000`




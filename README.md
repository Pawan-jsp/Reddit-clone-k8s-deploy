# Reddit-clone-k8s-deploy

Reddit Clone App on Kubernetes with Ingress
This project demonstrates how to deploy a Reddit clone app on Kubernetes with Ingress and expose it to the world using Minikube as the cluster.

Prerequisites
Before you begin, you should have the following tools installed on your local machine:

Docker
Kubeatm master and worker node
kubectl
Git
You can install Prerequisites by doing this steps. click here & complete all steps one by one.

Installation
Follow these steps to install and run the Reddit clone app on your local machine:

Clone this repository to your local machine: git clone https://github.com/LondheShubham153/reddit-clone-k8s-ingress.git
Navigate to the project directory: cd reddit-clone-k8s-ingress
Build the Docker image for the Reddit clone app: docker build -t reddit-clone-app .
Deploy the app to Kubernetes: kubectl apply -f deployment.yaml
Deploy the Service for deployment to Kubernetes: kubectl apply -f service.yaml
Enable Ingress by using Command: minikube addons enable ingress
Expose the app as a Kubernetes service: kubectl expose deployment reddit-deployment --type=NodePort --port=5000
Create an Ingress resource: kubectl apply -f ingress.yaml
Test Ingress DNS for the app:
Contributing
If you'd like to contribute to this project, please open an issue or submit a pull request.
# Reddit-clone-k8s-deploy

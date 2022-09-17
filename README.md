# Project 3
## Refactor Monolith to Microservice

### In this project a monolith infrastructure is refactored into a microservice, some of the core steps include;
- Splitting the backend api service into two independent services (api-feed and api-user)
- Setting up each microservice to be run in its own Docker container
- Setting up a Travis CI pipeline to push images to Dockerhub
- Setting up a kubernete cluster using aws eks
- Deploying the Dockerhub images to the Kubernetes cluster

### As a requirement for my project submission, i included the following screenshots in the screenshot directory
### Deployment Pipeline
* DockerHub showing containers that you have pushed
* GitHub repository’s settings showing your Travis webhook

### Kubernetes
* To verify Kubernetes pods are deployed properly
```bash
kubectl get pods
```
* To verify Kubernetes services are properly set up
```bash
kubectl describe services
```
* To verify that you have horizontal scaling set against CPU usage
```bash
kubectl describe hpa
```
* To verify that you have set up logging with a backend application
```bash
kubectl logs {pod_name}
```

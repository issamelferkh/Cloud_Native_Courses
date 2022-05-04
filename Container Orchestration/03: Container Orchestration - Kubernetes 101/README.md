# Container Orchestration - Kubernetes 101

## Why Container Orchestration
- Dev (Local) vs Prod (Cloud)
  - Localhost
    - Run container with older way: `sudo docker run -dp 3000:3000 issamelferkh/sample-app:1.0`

- Production
  - Generally use IaC
    - To create Container copies in multiple systems: Need to setup: Instances (systems) + Conf LB + Conf SG
      - Run containers with random ports: `sudo docker run -dp 3000 issamelferkh/sample-app:1.0`

- Issue:
  - In Cloud we can't pre-config security group or load balancer before cuz we can't know the rundom ports
  - Need run containers -> list open ports ->  re-conf sec group + load balancer
  - In case restart containers -> they take other random ports

- Solution:
  - Need and external tool -> that can listen and understand: the platform + open ports + running containers ...
  - Container Orchestration Platform

## Intro to Kubernetes
### What is Kubernetes:
- Open source container orchestration platform
- Developed by Google
- Helps manage containers in diff env (Physical machines, VM, Clouds)

### Kubernetes Architecture:




## Main K8s Components
### Node & Pod
### Service & Ingress
### ConfigMap & Secret
### Volume
### Deployment & StatefulSet

## Local Setup
### Kubernetes Configuration
### Minikube and Kubectl
### Setup K8s cluster locally

## Demo Project

## Resources
Resources: https://kube.academy/courses/kubernetes-101
Resources: https://www.youtube.com/watch?v=s_o8dwzRlu4

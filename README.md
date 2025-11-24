🤖 Three-Tier Microservice Application Deployment (Robot Shop)
🎯 Project Overview
This project involved deploying Robot Shop, a three-tier e-commerce application comprising 10+ distinct microservices (web, cart, payment, catalogue, etc.). The goal was to build a resilient, scalable cloud-native environment on AWS EKS.

🛠️Contribution and Key Achievements
I successfully implemented a cloud-native deployment pipeline and resolved critical infrastructure challenges:

Containerization: Used Docker to containerize all 10+ microservices, ensuring portability and consistency.

Orchestration (Helm): Employed and customized Helm charts to deploy the complex microservice architecture efficiently, replacing the need for extensive manual Kubernetes YAML management.

Persistent Storage (EKS/CSI/IRSA): Solved a critical deployment failure (stuck PVCs) by installing the AWS EBS CSI Driver add-on and configuring IAM Roles for Service Accounts (IRSA) for dynamic EBS volume provisioning (inspired by Abhishek Veeramalla's tutorials).

External Access (ALB/Ingress): Provisioned a public-facing Application Load Balancer (ALB) via the AWS Load Balancer Controller and a Kubernetes Ingress resource to ensure reliable public access and HTTP routing.

☁️ AWS EKS Deployment
Amazon EKS was selected for its scalable and highly available Kubernetes control plane. The entire cluster infrastructure and lifecycle were managed using the eksctl CLI tool.
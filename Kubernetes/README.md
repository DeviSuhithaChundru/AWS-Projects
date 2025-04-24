# Kubernetes Series – Part 1: Launch a Kubernetes Cluster Using Amazon EKS

This project is the first part of my Kubernetes hands-on learning series. In Part 1, I set up a fully managed Kubernetes cluster using Amazon EKS, automated via `eksctl`, and deployed with supporting AWS infrastructure including EC2, IAM, and CloudFormation.

---

## 🚀 Project Overview

This project demonstrates the complete setup of a Kubernetes environment on AWS. I used an EC2 instance to run `eksctl`, which generated the CloudFormation stacks necessary to provision the Amazon EKS control plane and node group. I configured IAM roles for secure access and tested cluster resilience by terminating nodes to observe Kubernetes' self-healing capabilities.

---
## 🛠️Tools & Technologies Used
- **Amazon Elastic Kubernetes Service (EKS)** – I used Amazon EKS as the managed Kubernetes service to deploy and scale containerized applications.
- **Amazon EC2** – I launched an EC2 instance to serve as the compute environment for running eksctl and managing the cluster setup.
- **AWS CloudFormation** – I utilized AWS CloudFormation to automate the provisioning of required infrastructure components.
- **AWS IAM**– I configured IAM roles and policies to securely manage access to AWS services during the deployment process.
- **Kubernetes** – I worked with Kubernetes as the container orchestration platform to manage workloads and services within the cluster.
- **eksctl** – I used the eksctl CLI tool to automate the creation and configuration of the EKS cluster.


---

---

## 🧭 Architecture Overview

A high-level view of the EKS cluster provisioning process:

1. Launched EC2 instance with IAM role
2. Installed `eksctl` 
3. Used `eksctl create cluster` to deploy EKS via CloudFormation
4. Created IAM Access Entries for EKS Console access
5. Simulated node failure and observe auto-recovery

![Architecture Diagram](Screenshots/Project_Architecture.png)

---

## 📸 Key Screenshots

You can view the full set of step-by-step screenshots here:  
[📂 Screenshots](https://github.com/DeviSuhithaChundru/AWS-Projects/tree/main/Kubernetes/Screenshots) *(link or folder)*

---

## 📚 Documentation

📄 [View Full Project Documentation](https://github.com/DeviSuhithaChundru/AWS-Projects/blob/main/Kubernetes/Kubernetes_EKS_Cluster%20Deployment.pdf)
This PDF includes:

- Project walkthrough
- CLI commands & IAM setup
- Cluster creation via eksctl
- CloudFormation stack analysis
- EKS access entries & console overview
- Node termination and auto-recovery test

---

## ✅ Key Takeaways

- Automated Kubernetes cluster setup using `eksctl`
- Gained experience in EKS architecture and RBAC configuration
- Explored AWS IAM, EC2, and CloudFormation in context of K8s
- Observed real-world use of self-healing infrastructure

---

## 🧹 Clean Up After Deployment

To avoid unnecessary resource costs, I:

- Deleted the EKS cluster using `eksctl delete cluster`
- Terminated associated EC2 instances
- Deleted leftover S3 and CloudFormation stacks

---

## 📬 Let's Connect

🔗 [LinkedIn](https://www.linkedin.com/in/suhithachundru/)  
🔗 [GitHub](https://github.com/DeviSuhithaChundru)

---



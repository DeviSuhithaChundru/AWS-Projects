# 📦 Kubernetes Series – Part 1: Launch a Kubernetes Cluster Using Amazon EKS

This is the first part of my Kubernetes hands-on learning series, where I explore how to set up and manage Kubernetes clusters across different platforms. In **Part 1**, I provisioned and deployed a production-ready Kubernetes cluster on AWS using Amazon EKS, EC2, IAM, and CloudFormation — all automated via `eksctl`.

---

# From EC2 to EKS: Automating Kubernetes Cluster Deployment

This project demonstrates how I provisioned and deployed a fully functional Kubernetes cluster on AWS using **Amazon Elastic Kubernetes Service (EKS)**, `eksctl`, and supporting services like EC2, IAM, and CloudFormation. The goal was to understand the complete lifecycle of Kubernetes infrastructure automation using real-world AWS tools.

---

## 🎯 Project Objective

The goal of this project was to automate the deployment of a production-ready Kubernetes cluster on AWS using **Amazon EKS**. Starting from an EC2 instance, I used `eksctl` to trigger an infrastructure-as-code workflow via **AWS CloudFormation**, which provisioned networking components, the EKS control plane, and managed node groups. I configured IAM roles and access entries to secure the environment, and finally validated the cluster’s resilience by simulating node failures. This hands-on project demonstrated my ability to integrate cloud-native tools, automate deployments, and implement secure, scalable Kubernetes infrastructure on AWS.

---

## 🏗 Architecture Overview

📌 ![Project Architecture](Project_Architecture.png)

---

## 🛠 Tech Stack

- **Tools Used**: AWS, EKS, EC2, IAM, CloudFormation, `eksctl`, `kubectl`  
- **Skills Applied**: Infrastructure as Code (IaC), Kubernetes Admin, Cloud Automation, IAM/RBAC, Resilience Testing

---

## 🔁 Cluster Resilience Test

To test Kubernetes' self-healing capabilities, I manually terminated EC2 nodes from the EKS-managed node group. Within minutes, Kubernetes automatically recreated the instances to restore the desired node count—proving the reliability and resilience of the system.

---

## 📸 Project Screenshots

You can view key screenshots that document each stage of the project in this 👉 [📂 Screenshots](#) *(replace with actual folder or link)*.

---

## 📚 What I Learned

- Automating Kubernetes cluster deployment with `eksctl`
- Configuring IAM roles and mapping to Kubernetes RBAC
- Using AWS CloudFormation behind `eksctl` for IaC
- Managing node groups, scaling, and auto-healing in Amazon EKS

---



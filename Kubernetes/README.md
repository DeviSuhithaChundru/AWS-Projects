# Kubernetes Series – Part 1: Launch a Kubernetes Cluster Using Amazon EKS

This is the first part of my Kubernetes hands-on learning series, where I explore how to set up and manage Kubernetes clusters across different platforms. In **Part 1**, I provisioned and deployed a production-ready Kubernetes cluster on AWS using Amazon EKS, EC2, IAM, and CloudFormation — all automated via `eksctl`.


# 🚀 From EC2 to EKS: Automating Kubernetes Cluster Deployment

This repository showcases the hands-on deployment of a Kubernetes cluster on AWS using **Amazon Elastic Kubernetes Service (EKS)**, `eksctl`, EC2, IAM, and CloudFormation.

---

## 🎯 Project Objective

The goal of this project was to provision and deploy a fully functional Kubernetes cluster on AWS using **Amazon Elastic Kubernetes Service (EKS)**. I launched an EC2 instance, configured IAM roles, and used `eksctl` to automate the provisioning process. The infrastructure was orchestrated through AWS CloudFormation. I secured access using IAM access entries and validated the cluster’s resilience by terminating nodes and observing Kubernetes' self-healing in action.

---

## 🏗 Architecture Overview

📌 *[Insert Architecture Diagram Here]*

---

## 🛠 Tools & Technologies

- **Amazon EKS** – Managed Kubernetes service
- **Amazon EC2** – Control environment for running eksctl
- **AWS IAM** – Role-based access control
- **AWS CloudFormation** – Infrastructure-as-Code provisioning
- **eksctl** – CLI tool to create and manage EKS clusters
- **kubectl** – Kubernetes command-line tool

---

## 🔁 Cluster Resilience Test

To test Kubernetes' self-healing capabilities, I manually terminated EC2 nodes from the EKS-managed node group. Within minutes, Kubernetes automatically recreated the instances to restore the desired node count—proving the reliability and resilience of the system.

---

## 📸 Project Screenshots

You can view key screenshots that document each stage of the project in this [📂 Screenshot Gallery](#) *(update with actual GitHub folder or hosted link)*.

---

## 📚 What I Learned

- How to automate Kubernetes cluster deployment using `eksctl`
- Setting up IAM roles and access entries for EKS
- How CloudFormation handles resource provisioning under the hood
- Managing node groups, scaling settings, and fault tolerance in Amazon EKS

---

## 👩‍💻 Author

**Devi Suhitha Chundru**  
📫 [LinkedIn](https://www.linkedin.com/in/your-profile)  
🌐 [Portfolio](https://your-portfolio.com) *(optional)*


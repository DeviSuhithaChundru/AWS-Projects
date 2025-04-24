# Kubernetes Series – Part 1: Launch a Kubernetes Cluster Using Amazon EKS

This project is the first part of my Kubernetes hands-on learning series. In Part 1, I set up a fully managed Kubernetes cluster using Amazon EKS, automated via `eksctl`, and deployed with supporting AWS infrastructure including EC2, IAM, and CloudFormation.

---

## 🚀 Project Overview

This project demonstrates the complete setup of a Kubernetes environment on AWS. I used an EC2 instance to run `eksctl`, which generated the CloudFormation stacks necessary to provision the Amazon EKS control plane and node group. I configured IAM roles for secure access and tested cluster resilience by terminating nodes to observe Kubernetes' self-healing capabilities.

---

## 🛠️ Tools & Technologies

- **Amazon Web Services (AWS)**
- **Amazon Elastic Kubernetes Service (EKS)**
- **Amazon EC2**
- **AWS CloudFormation**
- **AWS IAM**
- **eksctl**
- **kubectl**


---

## 📁 Project Structure

```
.
├── README.md
├── Project_Architecture.png
├── screenshots/
│   ├── ec2_instance.png
│   ├── eksctl_command.png
│   ├── cloudformation_stack.png
│   ├── eks_cluster_console.png
│   ├── node_termination.png
├── Kubernetes_EKS_Cluster_Deployment.pdf
```

---

## 🧭 Architecture Overview

A high-level view of the EKS cluster provisioning process:

1. Launch EC2 instance with IAM role
2. Install `eksctl` and `kubectl`
3. Use `eksctl create cluster` to deploy EKS via CloudFormation
4. Create IAM Access Entries for EKS Console access
5. Simulate node failure and observe auto-recovery

📌 *See [Screenshots/Project_Architecture.png] for visual flow*

---

## 📸 Key Screenshots

You can view the full set of step-by-step screenshots here:  
📂 [Screenshots Folder](#) *(link or folder)*

---

## 📚 Documentation

📄 **[Kubernetes_EKS_Cluster_Deployment.pdf](#)**  
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

🔗 [LinkedIn](https://www.linkedin.com/in/your-profile)  
🔗 [GitHub](https://github.com/DeviSuhithaChundru)

---



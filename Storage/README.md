**<h1><p align="center">🌍 Hosting a Static Website on Amazon S3</p></h1>**
## 📌 Project Overview
This project walks you through the process of hosting a fully functional static website using **Amazon S3 (Simple Storage Service)**. By leveraging AWS S3, you can deploy a scalable, secure, and cost-effective website without the need for traditional web servers.
This guide covers everything from setting up an S3 bucket, enabling static website hosting, configuring bucket policies for public access, handling errors.

## 🚀 Why Use Amazon S3 for Hosting?  
✔️ **Low Cost** – Only pay for storage and bandwidth, eliminating server costs.  
✔️ **High Availability** – AWS ensures global uptime and redundancy.  
✔️ **Scalability** – Handles any amount of web traffic effortlessly.  
✔️ **Security & Access Control** – Fine-grained permission management.  
✔️ **Custom Domain & HTTPS Support** – Secure access via SSL/TLS.  
✔️ **Seamless Content Delivery** – Improve speed using AWS CloudFront (CDN). 

## 🛠️ Tech Stack  
- **Amazon S3** – Object storage and static website hosting.  
- **AWS IAM** – Security and access policies.  
- **HTML, CSS, JavaScript** – Frontend for the website.  

## 🏗️ Setup & Deployment Guide  

### 🔹 Step 1: Create an Amazon S3 Bucket  
1. Log in to **AWS Console**.  
2. Navigate to **Amazon S3** → Click on **Create Bucket**.  
3. Enter a **unique Bucket Name** (e.g., `your-website-name`).  
4. Choose a **Region** (closest to your users for better speed).  
5. Disable **Block Public Access** (Required for public websites).  
6. Click **Create Bucket**.
 
### 🔹 Step 2: Enable Static Website Hosting  
1. Open the **created S3 Bucket**.  
2. Go to the **Properties tab** → Scroll down to **Static Website Hosting**.  
3. **Enable** it and set.

### 🔹 Step 3: Upload Website Files  
1. Click on the **Objects tab** in the **S3 bucket**.  
2. Upload your **HTML, CSS, JavaScript, and image files**.  
3. Click **Upload**.

### 🔹 Step 4: Configure Bucket Permissions  
1. Open the **Permissions** tab.  
2. Click **Edit Bucket Policy** and add the following JSON:  

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadGetObject",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::your-bucket-name/*"
    }
  ]
}



**<h1><p align="center">🌍 Hosting a Static Website on Amazon S3</p></h1>**
**📌 Project Overview**
This project walks you through the process of hosting a fully functional static website using **Amazon S3 (Simple Storage Service)**. By leveraging AWS S3, you can deploy a scalable, secure, and cost-effective website without the need for traditional web servers.
This guide covers everything from setting up an S3 bucket, enabling static website hosting, configuring bucket policies for public access, handling errors.

🚀 Why Use Amazon S3 for Hosting?
✅ Low Cost – Only pay for storage and bandwidth, eliminating server costs
✅ High Availability – AWS ensures global uptime and redundancy
✅ Scalability – Handles any amount of web traffic effortlessly
✅ Security & Access Control – Fine-grained permission management
✅ Custom Domain & HTTPS Support – Secure access via SSL/TLS
✅ Seamless Content Delivery – Improve speed using AWS CloudFront (CDN)

**🛠 Tech Stack**
**Amazon S3** – Object storage and static website hosting
**AWS IAM** – Security and access policies
**HTML, CSS, JavaScript** – Frontend for the website
**🔧 Setup & Deployment Guide**
**Step 1: Create an Amazon S3 Bucket**
1️⃣ Log in to AWS Console
2️⃣ Navigate to Amazon S3 → Click on Create Bucket
3️⃣ Enter a unique Bucket Name (e.g., nextwork-website-projectname)
4️⃣ Choose a Region (closest to your users for better speed)
5️⃣ Disable Block Public Access (Required for public websites)
6️⃣ Click **Create Bucket**

**Step 2: Enable Static Website Hosting**
1️⃣ Open the created S3 Bucket
2️⃣ Go to the Properties tab → Scroll down to Static website hosting
3️⃣ Enable it and set:

**Step 3: Upload Website Files**
1️⃣ Click on the Objects tab in the S3 bucket
2️⃣ Upload your HTML, CSS, JavaScript,image files and index.html
3️⃣ Click Upload

Step 4: Configure Permissions for Public Access
1️⃣ Open the Permissions tab
2️⃣ Under Bucket Policy, add the following JSON policy to allow public access:

json
Copy
Edit
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
3️⃣ Replace "your-bucket-name" with the actual bucket name
4️⃣ Click Save changes
**Step 5: Access Your Website**
🔗 Copy and paste the Bucket Website Endpoint URL in a browser to access your hosted website! 🎉
**📌 Future Enhancements**
🔹 Add CloudFront for improved performance & caching.
🔹 Implement HTTPS using an SSL certificate (via AWS Certificate Manager).
🔹 Enable logging & monitoring with AWS CloudWatch.
**🤝 Contributing**
Have ideas for improvement? Feel free to fork this repository and submit a pull request!
**📩 Contact & Support**
If you have any questions, feel free to reach out! 🚀



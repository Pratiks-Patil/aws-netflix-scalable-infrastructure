# 🎬 CloudFlix – Scalable Streaming Infrastructure on AWS

<p align="center">
  <img width="1881" height="836" alt="ChatGPT Image Jun 30, 2026, 12_31_01 PM" src="https://github.com/user-attachments/assets/2af35c3b-d401-4e57-a9b4-802a4d48d288" />

</p>

<p align="center">
  <strong>A Netflix-inspired streaming platform deployed on AWS to demonstrate scalable, highly available, and production-inspired cloud infrastructure using Amazon EC2, Application Load Balancer, Auto Scaling Groups, Amazon EBS, IAM, and Nginx.</strong>
</p>

<p align="center">

![AWS](https://img.shields.io/badge/AWS-Cloud-orange?style=for-the-badge&logo=amazonaws)
![EC2](https://img.shields.io/badge/Amazon-EC2-FF9900?style=for-the-badge&logo=amazonec2)
![ALB](https://img.shields.io/badge/Application-Load_Balancer-8C4FFF?style=for-the-badge)
![Auto Scaling](https://img.shields.io/badge/Auto-Scaling-blue?style=for-the-badge)
![EBS](https://img.shields.io/badge/Amazon-EBS-green?style=for-the-badge)
![Nginx](https://img.shields.io/badge/Nginx-Web_Server-009639?style=for-the-badge&logo=nginx)

</p>

---

# 📖 Project Overview

CloudFlix is a Netflix-inspired static streaming platform deployed on **Amazon Web Services (AWS)** to demonstrate the implementation of core cloud infrastructure concepts.

The project focuses on designing and deploying a scalable web application using industry-standard AWS services such as **Amazon EC2, Elastic Load Balancer (ALB), Auto Scaling Groups, Amazon EBS, IAM, Security Groups, and Nginx**.

Rather than focusing only on frontend development, this project showcases how a web application can be hosted using a production-inspired AWS architecture with scalability, availability, and infrastructure best practices in mind.

---

# 🏗 AWS Architecture

<p align="center">
<img width="1536" height="1024" alt="architecture" src="https://github.com/user-attachments/assets/b9317ea9-36c9-4a79-b543-1b7febff19c5" />

</p>

---

# ⚙ Architecture Workflow

```text
                    User
                      │
                  Internet
                      │
        Application Load Balancer
                      │
              Target Group
                      │
         Auto Scaling Group
                      │
          Amazon EC2 (Ubuntu)
                      │
                  Nginx Server
                      │
               CloudFlix Website
                      │
                 Amazon EBS
```

---

# ☁ AWS Services Used

| AWS Service | Purpose |
|-------------|---------|
| Amazon EC2 | Hosts the CloudFlix application |
| Amazon EBS | Persistent block storage for EC2 |
| Application Load Balancer | Distributes incoming HTTP traffic |
| Target Group | Routes traffic to healthy EC2 instances |
| Auto Scaling Group | Maintains desired number of instances |
| IAM | Secure AWS resource access |
| Security Groups | Network-level firewall configuration |
| Ubuntu Server | Operating System |
| Nginx | Web Server |

---

# ✨ Features

- 🎬 Netflix-inspired responsive UI
- ☁ Hosted on Amazon EC2
- ⚡ Nginx Web Server
- 💾 Persistent storage using Amazon EBS
- 🌐 Application Load Balancer integration
- 🎯 Target Group based request routing
- 📈 Auto Scaling Group configuration
- 🔐 IAM and Security Groups
- 📱 Fully Responsive Design
- 📊 Infrastructure Status Dashboard

---

# 📁 Repository Structure

```text
aws-netflix-scalable-infrastructure
├── deployment/
│   ├── 01-EC2-Deployment.md
│   ├── 02-EBS-Setup.md
│   ├── 03-Application-Load-Balancer.md
│   └── 04-Auto-Scaling-Group.md
│
├── index.html
├── style.css
├── script.js
├── README.md
└── LICENSE
```

---

# 📸 Project Screenshots

## 🏠 Homepage

<p align="center">
<img src="https://github.com/user-attachments/assets/398c9a8c-16c1-4471-aa3c-87d7709f5799" width="100%">
</p>

---

## 🌐 Website Access via ALB

<p align="center">
<img src="https://github.com/user-attachments/assets/81c04e7e-c6b5-48f0-92cb-493796b1dfc8" width="100%">
</p>

---

## ☁ EBS Volume Atatchment to Instance 

<p align="center">
<img width="1067" height="480" alt="Attach_Volume" src="https://github.com/user-attachments/assets/96de0314-32ed-4f42-bf9b-cc40ef67481f" />

</p>

---

## ⚖ Application Load Balancer

<p align="center">
<img src="https://github.com/user-attachments/assets/21b4aee8-0f4c-4128-9402-3cc1dd3ddfbb" width="100%">
</p>

---

## 📈 Auto Scaling Group

<p align="center">
<img src="https://github.com/user-attachments/assets/c8f04e4c-76c0-4bb1-a622-bcd887375c9d" width="100%">
</p>

---

## 💾 Amazon EBS

<p align="center">
<img src="https://github.com/user-attachments/assets/19ca9507-9d29-4708-be89-18195385859b" width="100%">
</p>

---

## 🔒 Verifying EBS from SSH

<p align="center">
<img src="https://github.com/user-attachments/assets/feb027a0-ec1f-441c-a1d9-0a3c116b19d0" width="100%">
</p>

---

## ✅ EBS Persistence Verification

<p align="center">
<img src="https://github.com/user-attachments/assets/c9291782-8432-4fbc-8f94-479e59b21c81" width="100%">
</p>

---

## 🚀 Launch Template

<p align="center">
<img src="https://github.com/user-attachments/assets/0bd04485-f7e6-4a37-95ed-b24ae7bef6df" width="100%">
</p>

---

## 🎯 Target Group

<p align="center">
<img src="https://github.com/user-attachments/assets/161f45b9-c173-4311-b8b0-8ffcfd7fb676" width="100%">
</p>
---

# 🚀 Deployment Summary

The project was deployed on AWS using the following workflow:

1. Created IAM user and configured secure access.
2. Launched an Ubuntu EC2 instance.
3. Configured Security Groups for HTTP and SSH.
4. Connected using SSH.
5. Installed and configured Nginx.
6. Deployed the CloudFlix frontend.
7. Attached an additional Amazon EBS volume.
8. Configured Application Load Balancer.
9. Created Target Group and health checks.
10. Created Launch Template.
11. Configured Auto Scaling Group.

---

# 📈 Future Enhancements

- CloudWatch Monitoring
- Route 53 Custom Domain
- AWS Certificate Manager (HTTPS)
- Amazon CloudFront CDN
- Amazon S3 for Static Assets
- GitHub Actions CI/CD
- Live AWS Infrastructure Dashboard
- Real-Time Monitoring using AWS SDK

---

# 📚 Learning Outcomes

This project demonstrates practical understanding of:

- AWS Cloud Fundamentals
- Amazon EC2
- Amazon EBS
- Application Load Balancer
- Target Groups
- Auto Scaling Groups
- IAM
- Security Groups
- Linux Administration
- Nginx Deployment
- Infrastructure Architecture

---

# 👨‍💻 Author

**Pratik Patil**

M.Tech Computer Engineering • VJTI Mumbai

GitHub: https://github.com/Pratiks-Patil

---

⭐ If you found this project helpful, consider giving it a star!

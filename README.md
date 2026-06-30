# 🎬 CloudFlix – Scalable Streaming Infrastructure on AWS

<p align="center">
  <img src="assets/images/banner.png" alt="CloudFlix Banner">
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
<img src="architecture/cloudflix-aws-architecture.png" width="100%">
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
│
├── assets/
│   ├── images/
│   ├── icons/
│   └── screenshots/
│
├── architecture/
│   └── cloudflix-aws-architecture.png
│
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

| Homepage | Infrastructure Dashboard |
|-----------|--------------------------|
| *Add Screenshot* | *Add Screenshot* |

| EC2 | ALB |
|-----|-----|
| *Add Screenshot* | *Add Screenshot* |

| Auto Scaling | EBS |
|--------------|-----|
| *Add Screenshot* | *Add Screenshot* |

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
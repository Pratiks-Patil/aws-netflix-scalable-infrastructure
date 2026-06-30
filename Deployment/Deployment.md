# 🚀 EC2 Deployment Guide

## Objective

Deploy the CloudFlix application on an Ubuntu EC2 instance using Nginx.

---

## AWS Services Used

- Amazon EC2
- IAM
- Security Groups
- Nginx
- SSH

---

## Steps Performed

### 1. Launch EC2 Instance

- Ubuntu Server 24.04 LTS
- Instance Type: t3.micro
- Key Pair created
- Security Group configured

---

### 2. Connect via SSH

```bash
ssh -i cloudflix-web-server-key.pem ubuntu@<EC2-PUBLIC-IP>
```

---

### 3. Update Server

```bash
sudo apt update
sudo apt upgrade -y
```

---

### 4. Install Nginx

```bash
sudo apt install nginx -y
```

---

### 5. Deploy Website

```bash
sudo cp -r * /var/www/html/
```

---

### 6. Restart Nginx

```bash
sudo systemctl restart nginx
```

---

## Verification

Open:

```
http://<EC2-PUBLIC-IP>
```

The CloudFlix homepage should load successfully.

---

## Outcome

Successfully deployed a Netflix-inspired streaming website on Amazon EC2 using Nginx.

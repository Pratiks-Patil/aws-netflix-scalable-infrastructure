# 🌐 Application Load Balancer Configuration

## Objective

Distribute incoming HTTP traffic across healthy EC2 instances.

---

## Components

- Application Load Balancer
- Target Group
- Health Checks
- Security Groups

---

## Steps Performed

### Create Target Group

- Target Type: Instance
- Protocol: HTTP
- Port: 80

---

### Register EC2 Instance

Added the running EC2 instance.

---

### Configure Health Check

Protocol:

```
HTTP
```

Path:

```
/
```

---

### Create Application Load Balancer

Configured:

- Internet Facing
- HTTP Listener
- Associated Target Group

---

## Verification

Opened:

```
http://<ALB-DNS>
```

Website loaded successfully.

---

## Outcome

Application Load Balancer successfully routed traffic to the CloudFlix EC2 instance.

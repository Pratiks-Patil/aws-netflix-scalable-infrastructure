# 📈 Auto Scaling Group Configuration

## Objective

Maintain application availability by automatically managing EC2 instances.

---

## Components

- Launch Template
- Auto Scaling Group
- Target Group

---

## Launch Template

Configured:

- Ubuntu Server
- t3.micro
- Security Group
- Key Pair

---

## Auto Scaling Configuration

Minimum Capacity

```
1
```

Desired Capacity

```
1
```

Maximum Capacity

```
2
```

---

## Target Group

Associated with:

```
CloudFlix Target Group
```

---

## Health Checks

Enabled:

- EC2
- ELB Health Checks

---

## Verification

Successfully launched the Auto Scaling Group.

Instances registered automatically with the Target Group.

---

## Outcome

CloudFlix infrastructure became highly available and ready for horizontal scaling.

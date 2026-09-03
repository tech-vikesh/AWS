# 🔐 Day 3 — AWS IAM (Identity & Access Management)

**Cohort:** AWS Cloud Cohort by CloudDevOpsHub Community

---

# 🎯 Today's Goal

Understand who can do what in your AWS account. Learn IAM users, permissions, account aliases, and build a Load Balancer with multiple EC2 instances.

By the end of today, you'll understand AWS Security Basics and High Availability Architecture. 🛡️

---

# 📚 Topics Covered

| # | Topic |
|---|--------|
| ✅ | AWS IAM Overview — Identity & Access Management Basics |
| ✅ | IAM Users & Service Access Configuration |
| ✅ | IAM Components — Users, Groups, Roles & Policies |
| ✅ | Load Balancers — Deep Dive & Architecture |
| ✅ | ALB, NLB & CLB — Types, Use Cases & Comparison |

---

# 🛠️ Daily Task — Practical Challenge

## ✔ Practical 1: Create IAM User with Limited Access

```text
Step 1: AWS Console → IAM → Users → Create User
Step 2: Username → "dev-user-01"
Step 3: Access Type → AWS Console Access
Step 4: Set Custom Password
Step 5: Attach Policy → AmazonEC2ReadOnlyAccess
Step 6: Create User → Download Credentials CSV
Step 7: Login with IAM User → Verify Limited Access
```

> ⚠️ Rule #1 in AWS Security: Never use the Root Account for daily work. Always use IAM Users.

---

## ✔ Practical 2: Create AWS Account Alias

### Create Professional Login URL

```text
Step 1: IAM → Dashboard → Account Alias → Create
Step 2: Set Alias → clouddevopshub-demo
Step 3: New Login URL:

https://clouddevopshub-demo.signin.aws.amazon.com/console

Step 4: Share this URL with IAM Users
```

> 💡 Interview Question: Why use an Account Alias?  
> Answer: It provides a professional and easy-to-remember login URL instead of using a 12-digit AWS Account ID.

---

## ✔ Practical 3: Create Application Load Balancer (ALB) with 2 EC2 Instances

### Architecture

```text
Internet
    │
    ▼
Application Load Balancer (Port 80)
    │
    ▼
Target Group
 ├── EC2-1 (App Server 1)
 └── EC2-2 (App Server 2)
```

### Configure EC2 Instances

```text
EC2-1:
<h1>Server 1 — Hello from AZ-1a</h1>

EC2-2:
<h1>Server 2 — Hello from AZ-1b</h1>
```

### ALB Setup

```text
Step 1: Launch 2 EC2 Instances
Step 2: Install Nginx on Both Servers
Step 3: EC2 → Load Balancers → Create Load Balancer
Step 4: Select Application Load Balancer (ALB)
Step 5: Select Both Availability Zones
Step 6: Create Target Group
Step 7: Register Both EC2 Instances
Step 8: Attach Target Group to ALB
Step 9: Create ALB
```

### Test Load Balancing

```text
Open ALB DNS URL in Browser
Refresh Multiple Times

Result:
Server 1
Server 2
Server 1
Server 2
```

✅ Traffic is distributed between both EC2 instances.

---

# 🎓 Key Learnings

- IAM controls access to AWS resources.
- Users, Groups, Roles, and Policies are the core IAM components.
- Root Account should be used only for account-level tasks.
- Account Alias creates user-friendly login URLs.
- Application Load Balancer distributes traffic across multiple servers.
- Load Balancers improve scalability and high availability.

---

# ✅ Outcome

Successfully created IAM users with restricted permissions, configured an AWS Account Alias, and deployed an Application Load Balancer with two EC2 instances.

Verified access control and traffic distribution across multiple servers.

🚀 Built a secure and highly available AWS architecture!

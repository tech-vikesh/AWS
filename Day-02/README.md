# 🖥️ Day 2 — AWS EC2 Deep Dive

**Cohort:** AWS Cloud Cohort by CloudDevOpsHub Community & Vikas Ratnawat

---

# 🎯 Today's Goal

Go deeper into EC2 by launching a Windows Server, configuring Nginx, deploying an HTML website, and setting up an Application Load Balancer (ALB).

By the end of today, you'll have a live website hosted on AWS! 🌐

---

# 📚 Topics Covered

| # | Topic |
|---|--------|
| ✅ | EC2 Instance Creation — Detailed Explanation & Use Cases |
| ✅ | EC2 Connection via Remote Desktop & Windows Server 2025 Setup |
| ✅ | EC2 Access using MobaXterm — Configuration & Connection |
| ✅ | Nginx Web Server Setup & HTML Website Deployment (Live Project) |
| ✅ | Application Load Balancer (ALB) — Traffic Distribution & High Availability |

---

# 🛠️ Daily Task — Practical Challenge

## ✔ Practical 1: Launch Windows Server 2025 EC2 Instance

```text
Step 1: EC2 → Launch Instance
Step 2: AMI → Windows Server 2025 Base
Step 3: Instance Type → t2.micro or t3.micro
Step 4: Key Pair → Use existing or create new
Step 5: Security Group → Allow RDP (port 3389) from My IP
Step 6: Launch → Get Password (using .pem key)
Step 7: Connect via RDP (Remote Desktop Protocol)
```

> 💡 **Pro Tip:** In interviews, always mention RDP = Port 3389 (Windows) and SSH = Port 22 (Linux).

---

## ✔ Practical 2: Nginx Web Server on Linux EC2 via MobaXterm

### Step 1 — Connect Using MobaXterm

```text
1. Download MobaXterm → https://mobaxterm.mobatek.net
2. New Session → SSH
3. Remote Host = EC2 Public IP
4. Use Private Key (.pem file)
5. Connect!
```

### Step 2 — Install Nginx

```bash
sudo yum update -y
sudo yum install nginx -y
sudo systemctl start nginx
sudo systemctl enable nginx
sudo systemctl status nginx
```

### Step 3 — Deploy HTML Website

```bash
cd /usr/share/nginx/html
sudo nano index.html
```

```html
<!DOCTYPE html>
<html>
<head>
<title>My AWS Website - Day 2</title>
</head>
<body>
  <h1>🚀 Hello from AWS EC2!</h1>
  <p>Deployed by [Your Name] — Day 2 of AWS Challenge</p>
  <p>Powered by Nginx on Amazon Linux | Tech Vikesh</p>
</body>
</html>
```

### Verify Website

```bash
curl http://localhost
```

Expected Result:

```text
You should see your HTML output.
```

### Access Website in Browser

```text
http://YOUR_EC2_PUBLIC_IP
```

> ⚠️ Make sure Port 80 (HTTP) is allowed in the Security Group before testing.

---

## ✔ Bonus: Application Load Balancer (ALB) Setup

```text
Step 1: Launch 2 EC2 Instances (same Nginx setup)
Step 2: EC2 → Load Balancers → Create Load Balancer
Step 3: Type → Application Load Balancer
Step 4: Scheme → Internet-facing
Step 5: Create Target Group → Add both EC2 Instances
Step 6: Create ALB → Copy DNS Name
Step 7: Access via ALB DNS → Traffic distributes between servers
```

> 💡 **Real-World Use Case:** Major platforms like Amazon, Flipkart, and Zomato use Load Balancers to distribute traffic across multiple servers. If one server becomes unavailable, the ALB automatically redirects traffic to healthy instances, ensuring high availability.

---

# ✅ Outcome

Successfully launched a Windows EC2 instance, connected through RDP, configured a Linux EC2 server using MobaXterm, installed Nginx, deployed a sample HTML website, and understood how Application Load Balancers improve scalability and high availability.

🚀 Website Successfully Hosted on AWS EC2!
``

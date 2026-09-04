# 🪣 Day 4 — AWS S3 + Online Portfolio (Static Website)

**Cohort:** AWS Cloud Cohort by CloudDevOpsHub Community

---

## 🎯 Today's Goal

Host your **resume/portfolio as a live website on AWS S3** for free!

This is one of the most interview-impressive projects a fresher can showcase. By the end of today, your resume will be live on the internet via AWS. 🌐

---

## 📚 Topics Covered

| # | Topic |
|---|--------|
| 🪣 | AWS S3 Overview — Simple Storage Service Explained |
| ❓ | What is S3 — Concepts, Use Cases & Benefits |
| 🛠️ | S3 Bucket Creation — Step-by-Step Hands-On |
| 🗂️ | Types of S3 Storage — Standard, Versioning, Lifecycle & More |

---

# 🛠️ Daily Task — Practical Challenge

## ✔ Practical 4: Host Your Resume/Portfolio on S3 (Static Website)

### Step 1 — Create S3 Bucket

```text
1. S3 → Create Bucket
2. Bucket Name → my-aws-resume-[yourname]
3. Region → ap-south-1 (Mumbai)
4. Uncheck "Block all public access"
5. Create Bucket
```

### Step 2 — Enable Static Website Hosting

```text
1. Open Bucket → Properties
2. Static Website Hosting → Enable
3. Index Document → index.html
4. Save Changes
```

### Step 3 — Create Your Resume HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Your Name | Cloud Engineer Resume</title>

  <style>
    body {
      font-family: Arial, sans-serif;
      max-width: 900px;
      margin: auto;
      padding: 20px;
      background: #f5f7fa;
      color: #333;
    }

    .container {
      background: white;
      padding: 25px;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }

    h1 {
      color: #232F3E;
    }

    h2 {
      color: #FF9900;
      border-bottom: 2px solid #FF9900;
      padding-bottom: 5px;
    }

    .badge {
      background: #232F3E;
      color: white;
      padding: 5px 12px;
      border-radius: 5px;
      display: inline-block;
      margin: 4px;
    }
  </style>
</head>

<body>

<div class="container">

  <h1>👋 Hi, I'm Your Name</h1>
  <p><strong>Cloud & DevOps Engineer | AWS Learner | CloudDevOpsHub Community</strong></p>

  <h2>🛠 Skills</h2>

  <span class="badge">AWS EC2</span>
  <span class="badge">AWS S3</span>
  <span class="badge">AWS IAM</span>
  <span class="badge">Linux</span>
  <span class="badge">Nginx</span>
  <span class="badge">Git</span>

  <h2>📋 Projects</h2>

  <ul>
    <li>Hosted Resume using AWS S3 Static Website Hosting</li>
    <li>Deployed Nginx Web Server on AWS EC2</li>
    <li>Configured IAM Users with Least Privilege Access</li>
  </ul>

  <h2>📚 Currently Learning</h2>

  <p>AWS 10-Day Cloud Challenge | CloudDevOpsHub Cohort-6</p>

  <h2>📧 Contact</h2>

  <p>Email: yourmail@example.com</p>
  <p>LinkedIn: https://linkedin.com/in/yourprofile</p>
  <p>GitHub: https://github.com/yourusername</p>

  <p style="color:gray;font-size:12px;">
    Hosted on AWS S3 | Built during AWS Cloud Challenge 🚀
  </p>

</div>

</body>
</html>
```

### Step 4 — Upload & Set Public Access

```text
1. Upload index.html to S3 Bucket
2. Configure Public Access Permissions
3. Copy Website Endpoint URL
4. Open URL in Browser
```

### Step 5 — Verify Website

✅ Resume Accessible via Internet

✅ Static Website Hosting Enabled

✅ AWS S3 Successfully Configured

---

## 🌐 Live Website

**Website URL:**  
https://your-bucket-name.s3-website.ap-south-1.amazonaws.com

---

## 📸 Screenshots

### S3 Bucket Created

images/s3-bucket.png

### Static Website Hosting Enabled

images/static-hosting.png

### Live Website

images/live-website.png

---

## 🏆 Challenge Completed

- ✅ Created S3 Bucket
- ✅ Enabled Static Website Hosting
- ✅ Uploaded HTML Resume
- ✅ Configured Public Access
- ✅ Verified Live Website

---

## 📊 S3 Quick Reference

| Feature | Detail |
|----------|----------|
| Storage Class | S3 Standard |
| Max Object Size | 5 TB |
| Bucket Naming | Globally Unique |
| Access Control | Bucket Policy / ACL |
| Use Cases | Static Websites, Backups, Data Lakes |

---

## 🚀 Learning Outcome

Successfully hosted a personal resume website using **AWS S3 Static Website Hosting**. Learned bucket creation, website hosting configuration, object permissions, public access management, and static website deployment on AWS.

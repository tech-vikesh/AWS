# 🪣 Day 4 — AWS S3 + Online Portfolio (Static Website)

**Cohort:** AWS Cloud Cohort by CloudDevOpsHub Community

---

## 🎯 Today's Goal

Host your **resume/portfolio as a live website on AWS S3** for free! This is one of the most interview-impressive things a fresher can show. By end of today, your resume will be live on the internet via AWS. 🌐

---

## 📚 Topics Covered

| # | Topic |
|---|---|
| 🪣 | AWS S3 Overview — Simple Storage Service Explained |
| ❓ | What is S3 — Concepts, Use Cases & Benefits |
| 🛠️ | S3 Bucket Creation — Step-by-Step Hands-On |
| 🗂️ | Types of S3 Storage — Standard, Versioning, Lifecycle & More |

---

## 🛠️ Daily Task — Practical Challenge

### ✔ Practical 4: Host Your Resume/Portfolio on S3 (Static Website)

### Step 1 — Create S3 Bucket:

```text
1. S3 → Create Bucket
2. Bucket name → "my-aws-resume-[yourname]" (must be globally unique)
3. Region → ap-south-1 (Mumbai)
4. Uncheck "Block all public access" → Confirm
5. Create Bucket
```

### Step 2 — Enable Static Website Hosting:

```text
1. Go to bucket → Properties tab
2. Scroll to "Static website hosting" → Enable
3. Index document → index.html
4. Save changes
```

### Step 3 — Create Your Resume HTML:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Your Name | Cloud Engineer Resume</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      max-width: 800px;
      margin: auto;
      padding: 20px;
    }

    h1 {
      color: #232F3E;
    }

    h2 {
      color: #FF9900;
      border-bottom: 2px solid #FF9900;
    }

    .badge {
      background: #232F3E;
      color: white;
      padding: 4px 10px;
      border-radius: 4px;
      margin: 3px;
      display: inline-block;
    }
  </style>
</head>

<body>

  <h1>👋 Hi, I'm Your Name</h1>
  <p>Cloud & DevOps Engineer | AWS Learner | CloudDevOpsHub Community</p>

  <h2>🛠️ Skills</h2>
  <span class="badge">AWS EC2</span>
  <span class="badge">AWS S3</span>
  <span class="badge">AWS IAM</span>
  <span class="badge">Linux</span>
  <span class="badge">Nginx</span>

  <h2>📋 Projects</h2>
  <ul>
    <li>Hosted this resume on AWS S3 Static Website Hosting</li>
    <li>Deployed Nginx Web Server on EC2 with Load Balancer</li>
    <li>Configured IAM users with least privilege access</li>
  </ul>

  <h2>📚 Currently Learning</h2>
  <p>AWS 10-Day Cloud Challenge | CloudDevOpsHub Cohort-6</p>

  <p style="color:gray; font-size:12px;">
    Hosted on AWS S3 | Built during 10-Day AWS Challenge 🚀
  </p>

</body>
</html>
```

### Step 4 — Upload & Set Public Access:

```text
1. Upload index.html to bucket
2. Select the file → Actions → Make Public via ACL
3. Copy the S3 Website URL from Properties
4. Open in browser — YOUR RESUME IS LIVE! 🎉
```

### Step 5 (Optional) — Add Route 53 Custom Domain:

```text
1. Route 53 → Create Hosted Zone
2. Add your domain (e.g., yourname.cloud)
3. Create A Record → Alias → S3 website endpoint
4. Access your resume at: http://yourname.cloud
```

---

## 🏆 Today's Challenge

### 🔥 CHALLENGE:

- Deploy your resume/portfolio on AWS S3
- Copy the live S3 URL
- Add the URL to your LinkedIn Profile → Contact Info → Website
- Post on LinkedIn with the live link!

---

## 📸 Screenshot Checklist

- ✅ S3 Bucket created with static hosting enabled
- ✅ index.html uploaded
- ✅ Live website URL from S3
- ✅ Resume visible in browser via S3 URL

---

## 📊 S3 Quick Reference

| Feature | Detail |
|----------|----------|
| Storage class | S3 Standard (default) |
| Max object size | 5 TB |
| Bucket naming | Globally unique, lowercase |
| Access control | Bucket Policy / ACL / Public Access Block |
| Use Cases | Backups, Static Sites, Data Lakes, Media Storage |

---

## 🌐 Live Website

**S3 Website URL:**  
`http://your-bucket-name.s3-website.ap-south-1.amazonaws.com`

---

## 🚀 Learning Outcome

Successfully hosted a resume/portfolio website using AWS S3 Static Website Hosting and learned bucket creation, object upload, public access configuration, and website hosting on AWS.
   

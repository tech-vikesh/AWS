☁️ Day 1 — AWS Introduction & EC2 Basics

# 🎯 Today's Goal
2
 
3
Get your AWS account live and launch your **first EC2 virtual machine** in the cloud.
4
 
5
By the end of today, you should have a running server on AWS. That's the mission. 💪
6
 
7
---
8
 
9
# 📚 Topics Covered
10
 
11
| # | Topic |
12
|---|-------|
13
| ✅ | History of AWS - How it all started in 2006 |
14
| ✅ | What is AWS - The World's #1 Cloud Platform |
15
| ✅ | Traditional IT vs Cloud Services - Why Cloud Wins |
16
| ✅ | AWS Global Infrastructure - Regions, AZs, Edge Locations |
17
| ✅ | AWS Account Creation - Free Tier Walkthrough |
18
| ✅ | First EC2 Instance Creation - Live Practical |
19
 
20
---
21
 
22
# 🛠️ Daily Task - Practical Challenge
23
 
24
## ✅ Task 1: Create Your AWS Free Tier Account
25
 
26
### Steps
27
 
28
1. Visit: https://aws.amazon.com/free
29
2. Sign up using your email address.
30
3. Add a credit/debit card for verification.
31
4. Select **Basic Support (Free)**.
32
5. Login to AWS Console.
33
 
34
🔗 https://console.aws.amazon.com
35
 
36
### 💡 Pro Tip
37
 
38
Use a dedicated email address for AWS and never share root account credentials.
39
 
40
---
41
 
42
## ✅ Task 2: Launch Your First EC2 Instance (Linux VM)
43
 
44
### Configuration
45
 
46
- **Instance Name:** My First Server
47
- **AMI:** Amazon Linux 2023 (Free Tier Eligible)
48
- **Instance Type:** t2.micro
49
- **Key Pair:** Create New Key Pair and Download `.pem` File
50
- **Security Group:** Allow SSH (Port 22) from My IP
51
 
52
### Steps
53
 
54
1. Navigate to **EC2 Dashboard**.
55
2. Click **Launch Instance**.
56
3. Enter instance name as **my-first-server**.
57
4. Select **Amazon Linux 2023 AMI**.
58
5. Choose **t2.micro** instance type.
59
6. Create a new key pair.
60
7. Configure security group.
61
8. Launch the instance.
62
9. Connect using **EC2 Instance Connect** (Browser SSH).
63
 
64
---
65
 
66
# 🖥️ Verification Commands
67
 
68
### Check Current User
69
 
70
```bash
71
whoami
72
```
73
 
74
**Output**
75
 
76
```bash
77
ec2-user
78
```
79
 
80
### Check Linux Kernel Version
81
 
82
```bash
83
uname -r
84
```
85
 
86
**Output**
87
 
88
```bash
89
Shows Linux kernel version
90
```
91
 
92
---
93
 
94
# ✅ Outcome
95
 
96
Successfully created an AWS Free Tier account and launched my first EC2 Linux virtual machine.
97
 
98
Verified instance access using EC2 Instance Connect and executed basic Linux commands successfully.
99
 
100
🚀 First AWS EC2 Server Deployed Successfully!

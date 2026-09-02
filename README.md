🎯 Today's Goal
Get your AWS account live and launch your first EC2 virtual machine in the cloud.
By end of today — you should have a running server on AWS. That's the mission. 💪

📚 Topics Covered
#	Topic
✅	History of AWS — How it all started in 2006
✅	What is AWS — The world's #1 Cloud Platform
✅	Traditional IT vs Cloud Services — Why Cloud wins
✅	AWS Global Infrastructure — Regions, AZs, Edge Locations
✅	AWS Account Creation — Free Tier walkthrough
✅	First EC2 Instance Creation — Live Practical
🛠️ Daily Task — Practical Challenge
✔ Task 1: Create Your AWS Free Tier Account
1. Go to → https://aws.amazon.com/free
2. Sign up with your email
3. Add credit/debit card (₹2 verification, not charged)
4. Select "Basic Support – Free"
5. Login to AWS Console → https://console.aws.amazon.com
💡 Pro Tip: Use a dedicated email for AWS. Never share root credentials.

✔ Task 2: Launch Your First EC2 Instance (Linux VM)
Step 1: Go to EC2 → Launch Instance
Step 2: Name it → "my-first-server"
Step 3: AMI → Amazon Linux 2023 (Free Tier Eligible)
Step 4: Instance Type → t2.micro (Free Tier)
Step 5: Key Pair → Create new → Download .pem file (SAVE IT!)
Step 6: Security Group → Allow SSH (port 22) from My IP
Step 7: Launch Instance
Step 8: Connect via EC2 Instance Connect (browser SSH)
Verify it works:

whoami
# Output: ec2-user

uname -r
# Shows Linux kernel version

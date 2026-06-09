🌐 Live Demo

👉 http://<YOUR-EC2-PUBLIC-IP>

⚠️ Replace <YOUR-EC2-PUBLIC-IP> with your actual instance IP

📌 Project Overview

This project demonstrates real-world cloud deployment of a static portfolio website on an AWS EC2 instance running RHEL 10, hosted using Apache HTTP Server.

It covers full lifecycle:

Cloud infrastructure setup
Linux server configuration
Web server deployment
Security configuration
🏗️ Architecture
☁️ AWS EC2 (RHEL 10)
🌐 Apache HTTP Server (httpd)
🔐 AWS Security Groups (HTTP + SSH)
💻 Static Frontend (HTML5)
⚙️ Tech Stack
AWS EC2
Red Hat Enterprise Linux 10
Apache Web Server
HTML5 / CSS3
SSH (Key-based authentication)
📂 Project Structure
portfolio-website-on-aws-rhel10/
│
├── index.html
├── README.md
│
└── screenshots/
    ├── ec2-instance.png
    ├── security-group.png
    └── homepage.png
🚀 Deployment Workflow
1️⃣ Launch EC2 Instance
AMI: RHEL 10
Instance Type: t2.micro (Free Tier)
Key Pair generated for SSH access
2️⃣ Connect via SSH
ssh -i "key.pem" ec2-user@<EC2-PUBLIC-IP>
3️⃣ Install Apache Server
sudo dnf update -y
sudo dnf install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd
4️⃣ Deploy Website
cd /var/www/html
sudo nano index.html

Paste your HTML code and save.

5️⃣ Configure Security Group

Allow inbound rules:

HTTP → Port 80
SSH → Port 22
🌍 Access Website

Once deployed:

http://<EC2-PUBLIC-IP>
📸 Screenshots
🖥️ EC2 Instance

🔐 Security Group Configuration

🌐 Website Homepage

📊 Key Learnings
AWS EC2 provisioning & management
Linux server administration (RHEL 10)
Apache HTTP server configuration
Cloud networking (Security Groups)
Real-world deployment pipeline
🚀 Future Improvements
🔒 Add HTTPS using SSL (Let’s Encrypt)
🌐 Attach custom domain (Route 53)
⚡ CI/CD pipeline using GitHub Actions
🐳 Docker-based deployment
⚖️ Load Balancer integration
🏆 Project Highlights
Production-style cloud deployment flow
Real server hosting (not local simulation)
Fully manual Linux + AWS configuration
Beginner → Intermediate DevOps foundation
👨‍💻 Author

Built as a hands-on cloud deployment project to strengthen:

AWS fundamentals
Linux system administration
Web hosting workflows
⭐ If you like this project

Give it a ⭐ on GitHub and feel free to fork it!

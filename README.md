🚀 AWS EC2 Web Server Deployment (RHEL 10 + Apache)








📌 Project Summary

A production-style deployment of a static portfolio website on AWS EC2 (RHEL 10) using Apache HTTP Server.
This project demonstrates cloud hosting, Linux server configuration, and basic DevOps workflow.

🌐 Live Deployment

👉 http://<EC2-PUBLIC-IP>

Replace <EC2-PUBLIC-IP> with your actual instance IP

🧱 System Architecture
User → AWS EC2 Instance → Apache Web Server → index.html (Website)
⚙️ Tech Stack
☁️ AWS EC2
🐧 Red Hat Enterprise Linux 10
🌐 Apache HTTP Server (httpd)
💻 HTML5
🔐 SSH (Key-based login)
📂 Project Structure
portfolio-website-on-aws-rhel10/
│
├── index.html
├── README.md
└── screenshots/
    ├── ec2-instance.png
    ├── security-group.png
    └── homepage.png
🚀 Deployment Workflow
1️⃣ Launch EC2 Instance
OS: RHEL 10
Type: t2.micro (Free Tier)
Key pair generated for SSH access
2️⃣ SSH Into Instance
ssh -i key.pem ec2-user@<public-ip>
3️⃣ Install Apache
sudo dnf update -y
sudo dnf install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd
4️⃣ Deploy Website
cd /var/www/html
sudo nano index.html

Paste your HTML code and save.

5️⃣ Configure Security Group

Inbound Rules:

HTTP (80) → Open to public
SSH (22) → Your IP only
🌍 Website Access
http://<EC2-PUBLIC-IP>
📸 Screenshots
🖥️ EC2 Instance

🔐 Security Group

🌐 Website Output

🎯 Key Learnings
AWS EC2 provisioning & management
Linux server administration (RHEL)
Apache web server configuration
Security group & network rules
Real-world deployment workflow
🚀 Future Enhancements
🔒 HTTPS using SSL (Let’s Encrypt)
🌐 Custom domain via Route 53
⚡ CI/CD pipeline using GitHub Actions
🐳 Docker container deployment
⚖️ Load balancer integration
🏆 Project Highlights
Real cloud deployment (not local simulation)
End-to-end server setup from scratch
Linux + AWS integration
Beginner → DevOps foundation project
👨‍💻 Author

Built as a hands-on cloud & Linux deployment project to strengthen AWS fundamentals and real-world system understanding.

⭐ Note

This project is part of my cloud learning journey and demonstrates practical AWS EC2 hosting.

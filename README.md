# AWS EC2 Web Server Deployment (RHEL 10 + Apache)

## 📌 Overview
Static website hosted on AWS EC2 using RHEL 10 and Apache HTTP Server.

---

## 🌐 Live Demo
http://<EC2-PUBLIC-IP>

---

## ⚙️ Tech Stack
AWS EC2 • RHEL 10 • Apache HTTP Server • HTML

---

## 🧱 Architecture
User → EC2 Instance → Apache → index.html

---

## 🚀 Deployment Steps

### 1. Install Apache
```bash

2. Deploy Website
cd /var/www/html
sudo nano index.html

3. Open Security Group
HTTP: 80
SSH: 22

📸 Screenshots
EC2 Instance → screenshots/ec2.png
Security Group → screenshots/security.png
Homepage → screenshots/home.png

🎯 Learnings

AWS EC2 • Linux basics • Apache setup • Networking fundamentals

👨‍💻 Author

AWS + Linux deployment practice project

sudo dnf install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd

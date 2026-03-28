# 🚀 Automated WordPress Hosting using Ansible (LEMP Stack on AWS)

## 📌 Project Overview

This project demonstrates how to **automate the deployment of a WordPress website** using **Ansible** on a **LEMP stack (Linux, Nginx, MariaDB, PHP)** hosted on an AWS EC2 instance.

The objective is to eliminate manual configuration and ensure a **secure, consistent, and production-ready deployment**.

---

## 🏗️ Architecture

User → Nginx → PHP-FPM → MariaDB
⬆
Ansible Automation (Control Node)

---

## ⚙️ Technologies Used

* AWS EC2 – Cloud hosting
* Linux (RHEL / Amazon Linux) – Operating system
* Ansible – Automation tool
* Nginx – Web server
* PHP-FPM – Backend processing
* MariaDB – Database
* WordPress – CMS
* phpMyAdmin – Database management
* SFTP – Secure file transfer
* Let’s Encrypt – SSL (HTTPS)
* Certbot – SSL automation tool
* Git & GitHub – Version control

---

## 🔧 Key Features

* Automated LEMP stack installation
* WordPress deployment with database integration
* Hosting website in user’s home directory (`/home/user/site/public`)
* phpMyAdmin accessible via `/phpmyadmin`
* Secure SFTP access using chroot jail
* Automated database and user creation
* **HTTPS enabled using Let’s Encrypt SSL** 🔒
* Automatic HTTP → HTTPS redirection
* Proper file permissions and security configuration
* Repeatable and scalable deployment

---

## 📂 Project Structure

```id="lbbhb8"
LEMP-STACK/
│
├── ansible.cfg
├── inventory
├── site.yml
├── ssl.yml
├── sftp.yml
├── requirements.yml
└── README.md
```

---

## 🚀 Workflow

### 1. Server Setup

* Launch EC2 instance
* Configure security groups (Ports 22, 80, 443)
* Connect using SSH

---

### 2. Install LEMP Stack

* Install Nginx
* Install PHP & PHP-FPM
* Install MariaDB

---

### 3. Ansible Automation

* Configure inventory and ansible.cfg
* Write playbooks
* Automate package installation and services

---

### 4. WordPress Deployment

* Download WordPress into `/home/{{ username }}/{{ site_name }}/public`
* Configure database
* Setup Nginx configuration

---

### 5. Database Configuration

* Create database (`wordpress`)
* Create user (`wp_user`)
* Grant privileges

---

### 6. phpMyAdmin Setup

* Install phpMyAdmin
* Configure access via `/phpmyadmin`
* Verify database connection

---

### 7. SSL Configuration (HTTPS) 🔒

* Install Certbot
* Generate SSL certificate using Let’s Encrypt
* Configure Nginx for HTTPS
* Enable automatic HTTP → HTTPS redirection
* Ensure secure communication

---

### 8. SFTP Configuration

* Create user
* Configure chroot directory
* Restrict access to home directory
* Enable secure file transfer

---

## 🌐 Access URLs

| Service         | URL                           |
| --------------- | ----------------------------- |
| Website (HTTP)  | http://<your-domain>            |
| Website (HTTPS) | https://<your-domain>         |
| phpMyAdmin      | http://<your-domain>/phpmyadmin |
| WordPress Admin | http://<your-domain>/wp-admin   |


---

## 🔐 Security

* HTTPS enabled using Let’s Encrypt
* Secure SSH access
* Chrooted SFTP environment
* Restricted user permissions
* Database access limited to specific user
* Nginx configured with least privilege

---

## 💡 Use Case

* Nginx → Handles HTTP/HTTPS requests
* PHP-FPM → Processes backend logic
* MariaDB → Stores application data
* Ansible → Automates deployment
* SSL → Secures communication
* SFTP → Secure file transfer

---

## 🎯 Outcome

* Fully automated and secure WordPress deployment
* Reduced manual effort
* Improved consistency and reliability
* Real-world DevOps implementation experience

---

## 📚 Learning

* Ansible automation
* Linux server management
* Web server configuration (Nginx)
* SSL setup and HTTPS configuration
* Secure file transfer (SFTP)
* DevOps best practices

---

## 🙌 Author

**Naja Fathima**
DevOps & Cloud Enthusiast 🚀

---


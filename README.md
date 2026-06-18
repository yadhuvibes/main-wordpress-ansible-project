# WordPress Hosting Automation using Ansible

## Project Overview

This project demonstrates the automated deployment and configuration of a WordPress hosting environment on an Amazon Linux server using Ansible.

The automation includes installation and configuration of Nginx, PHP, MariaDB, phpMyAdmin, SFTP access, SSL certificate generation using Let's Encrypt, and WordPress setup with a custom domain.

---

# Features

* Automated installation of Nginx
* Automated installation of PHP 8+
* Automated installation and configuration of MariaDB
* WordPress deployment
* phpMyAdmin integration
* SFTP user configuration
* Custom website directory under `/home`
* HTTPS enabled using Let's Encrypt SSL
* Domain configuration
* Infrastructure automation using Ansible roles

---

# Project Structure

```
main-wordpress-ansible-project/

├── inventory/
├── playbooks/
│   └── site.yml
├── roles/
│   ├── nginx/
│   ├── php/
│   ├── mysql/
│   ├── sftp/
│   └── wordpress/
├── group_vars/
├── host_vars/
└── README.md
```

---

# Technologies Used

* Ansible
* Nginx
* PHP 8+
* MariaDB
* WordPress
* phpMyAdmin
* OpenSSH (SFTP)
* Let's Encrypt (Certbot)
* Linux (Amazon Linux)

---

# Project Objectives

* Automate web server provisioning.
* Configure secure SFTP access.
* Host a WordPress website.
* Enable secure HTTPS communication.
* Provide database management through phpMyAdmin.
* Demonstrate Infrastructure as Code (IaC) using Ansible.

---

# Project Workflow

1. Configure Ansible control node.
2. Install Nginx.
3. Install PHP and PHP-FPM.
4. Install MariaDB.
5. Create website user.
6. Create website directory structure.
7. Configure SFTP.
8. Configure phpMyAdmin.
9. Deploy WordPress.
10. Configure custom domain.
11. Install SSL certificate.
12. Customize WordPress.
13. Publish personal blog.

---

# Website Directory Structure

```
/home/<website_user>/<website_name>/public
```

Example:

```
/home/wordpressuser/myblog/public
```

---

# Ansible Roles

## nginx

* Install Nginx
* Enable service
* Start service
* Deploy configuration

## php

* Install PHP packages
* Configure PHP-FPM
* Enable PHP-FPM

## mysql

* Install MariaDB
* Create WordPress database
* Create database user

## sftp

* Create website user
* Configure SFTP
* Configure directory permissions

## wordpress

* Deploy WordPress
* Configure wp-config.php
* Connect to database

---

# Security Features

* HTTPS using Let's Encrypt SSL
* SFTP-only user access
* Database authentication
* Secure file permissions
* Nginx reverse proxy configuration

---

# URLs

## Website

```
https://your-domain-name
```

## WordPress Admin

```
https://your-domain-name/wp-admin
```

## phpMyAdmin

```
https://your-domain-name/phpmyadmin
```

---

# Credentials

## SFTP

* Host: <Server IP>
* Username: <Configured User>
* Password/SSH Key: <Configured Credential>

## phpMyAdmin

* URL: https://your-domain-name/phpmyadmin
* Username: <Database User>
* Password: <Database Password>

## WordPress

* URL: https://your-domain-name/wp-admin
* Username: <Admin Username>
* Password: <Admin Password>

---

# Deployment

Clone the repository:

```bash
git clone <repository-url>
cd main-wordpress-ansible-project
```

Run the playbook:

```bash
ansible-playbook playbooks/site.yml
```

Verify services:

```bash
systemctl status nginx
systemctl status php-fpm
systemctl status mariadb
```

---

# Verification Checklist

* Nginx running
* PHP-FPM running
* MariaDB running
* WordPress accessible
* phpMyAdmin accessible
* HTTPS enabled
* SFTP working
* WordPress admin login successful
* Blog published successfully

---

# Learning Outcomes

* Infrastructure as Code with Ansible
* Web server automation
* Linux server administration
* WordPress deployment
* Database management
* SSL configuration
* SFTP configuration
* Domain hosting
* Nginx configuration
* DevOps fundamentals

---

# Future Enhancements

* Docker-based deployment
* CI/CD pipeline integration
* Automated backups
* Monitoring with Prometheus and Grafana
* Load balancing
* Auto-scaling
* Multi-site WordPress deployment

---

# Author

**Yadhukrishna P. R.**

DevOps | Linux | Cloud | Automation | Ansible | AWS


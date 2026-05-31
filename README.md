# Ansible Web Server

![Ansible](https://img.shields.io/badge/Ansible-FF6600?style=for-the-badge&logo=ansible&logoColor=white)
![Nginx](https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white)

A **beginner-friendly** Ansible project that turns a fresh machine into a working web server and deploys a custom homepage.

## 🎯 Objective

Use Ansible to:

- Install and configure Nginx
- Deploy a static website from `index.html`
- Maintain idempotent and repeatable provisioning

## ✨ Features

- Installs Nginx on the target host
- Copies a custom homepage to the web server root
- Uses an inventory and a simple playbook
- Safe to run multiple times without breaking the server

## 📋 Project Structure

```text
ansible-webserver/
├── README.md
├── inventory.ini
├── playbook.yml
├── index.html
├── ansible.cfg
└── .gitignore
```

## 🚀 Quick Start

### 1. Clone the repository

```bash
git clone https://github.com/tinobrace/ansible-webserver.git
cd ansible-webserver
```

### 2. Run the Ansible playbook

```bash
ansible-playbook -i inventory.ini playbook.yml
```

### 3. Open the web page

Visit:

- `http://localhost`
- or `http://<your-server-ip>/ 192.168.100.50`

You should see the deployed welcome page.

## 🛠️ What’s included

- `playbook.yml` — the Ansible playbook that installs Nginx and deploys `index.html`
- `inventory.ini` — the target host inventory file
- `ansible.cfg` — optional Ansible configuration
- `index.html` — the static homepage deployed to Nginx

## 💡 Practice Exercises

1. Edit `index.html` and re-run the playbook.
2. Add a task to install `curl`.
3. Extend the playbook to create `/etc/motd` with a welcome message.
4. Deploy the playbook to a real VPS (DigitalOcean, AWS, etc.).

# Ansible Web Server

A simple beginner-friendly Ansible project.

## 🎯 Objective
Automatically turn a server into a web server that displays a nice "Hello Students!" page using **Ansible**.

## 📋 Project Structure

ansible-webserver/
├── README.md
├── inventory.ini
├── playbook.yml
├── index.html
├── ansible.cfg
└── .gitignore


## 🚀 How to Use

### Step 1: Clone or Download
```bash
git clone <your-repo-url>
cd ansible-webserver-tutorial

### Step 2: Test on Your Local Machine
```bash
ansible-playbook -i inventory.ini playbook.yml

### Step 3: View the Result
```bash
Open your browser and go to: http://localhost or http://your-server-ip
You should see a beautiful welcome page!


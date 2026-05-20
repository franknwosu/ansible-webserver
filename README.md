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
git clone https://github.com/tinobrace/ansible-webserver.git
cd ansible-webserver

### Step 2: Run the playbook
```bash
ansible-playbook -i inventory.ini playbook.yml

### Step 3: View the Result
```bash
Open your browser and go to: http://localhost or http://your-server-ip
You should see a beautiful welcome page!

## Practice Exercises

1. Change the message in `index.html` and re-run the playbook
2. Add a new task to install `curl`
3. Modify the playbook to create a file `/etc/motd` with a welcome message
4. Fork this repo and try deploying it on a real VPS (DigitalOcean, AWS, etc.)

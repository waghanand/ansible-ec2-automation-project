# Ansible EC2 Automation Project

## 📌 Project Overview

This project demonstrates how to use Ansible to connect to and manage Ubuntu EC2 instances on AWS through SSH. It covers inventory configuration, SSH authentication, and remote server connectivity testing.

## 🎯 Objectives

- Configure an Ansible control node and managed EC2 instance.
- Establish SSH connectivity between EC2 instances.
- Define hosts and connection variables in an Ansible inventory.
- Test connectivity using the Ansible ping module.
- Execute commands on remote Linux servers.

## 🛠️ Technologies Used

- **AWS EC2** — Cloud virtual machines
- **Ubuntu Linux** — Operating system
- **Ansible** — Configuration management and automation
- **SSH** — Secure remote access
- **Git and GitHub** — Version control and project hosting

## 📂 Project Structure

```text
ansible-project/
├── .gitignore
├── inventory.ini
└── README.md
```

## ⚙️ Configuration

1. Install Ansible on the control node.
2. Configure SSH access to the target EC2 instance.
3. Create an inventory file listing the managed hosts.
4. Configure the SSH username, private key path, and Python interpreter.
5. Ensure network rules allow SSH traffic between the instances.

## ▶️ Commands Used

Check the Ansible version:

```bash
ansible --version
```

Check inventory configuration:

```bash
ansible-inventory -i inventory.ini --list
```

Test connectivity:

```bash
ansible web1 -i inventory.ini -m ping
```

Execute a remote command:

```bash
ansible web1 -i inventory.ini -m command -a "hostname"
```

A successful ping returns `pong`.

## 🔐 Security

- Never upload private SSH keys (`.pem`) to GitHub.
- Keep credentials and sensitive configuration out of public repositories.
- Restrict SSH access through appropriate AWS security group rules.
- Review inventory details before publishing a public repository.

## 📚 Learning Outcomes

- Understanding Ansible inventory files.
- Connecting to AWS EC2 instances using SSH.
- Running Ansible ad-hoc commands.
- Troubleshooting SSH authentication and inventory errors.
- Publishing DevOps projects using Git and GitHub.

## 👨‍💻 Author

**Anand Wagh**

GitHub: [@waghanand](https://github.com/waghanand)


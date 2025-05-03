# Automation with Ansible Assignment.

## Overview

This assignment uses Ansible to automate the deployment of a simple Flask application across multiple web servers. HAProxy is used to distribute incoming traffic among these servers for basic load balancing.

## Components

- **Flask App**: A lightweight Python application that returns the hostname and current time.
- **Web Servers**: Hosts running the Flask app.
- **HAProxy**: Acts as a load balancer, distributing requests across the web servers.
- **Bastion Host**: Used as a secure jump host to access internal servers.

## Files Included

- `site.yaml` – The main Ansible playbook that installs and configures HAProxy and the Flask application.
- `hosts` – Ansible inventory file that defines the target servers.
- `app.py` – The Flask application file.
- `README.md` – Project documentation.

## How to Run
```bash
ansible-playbook -i hosts site.yaml

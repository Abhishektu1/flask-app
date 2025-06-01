# Flask App with Ubuntu CIS Hardening Automation

This repository contains a simple Flask web application along with an Ansible playbook to create a hardened Ubuntu AMI by applying basic CIS (Center for Internet Security) controls.

---

## Project Structure

- `app.py`  
  A simple Flask application.

- `requirements.txt`  
  Python dependencies for the Flask app.

- `Dockerfile`  
  Dockerfile to containerize the Flask app.

- `.github/workflows/deploy.yml`  
  GitHub Actions workflow file to automate deployment.

- `cis_hardening.yml`  
  Ansible playbook to automate Ubuntu server hardening based on CIS benchmarks.

- `inventory`  
  Ansible inventory file with target hosts.

---

## Features

### Flask App

- Basic web application built with Flask.
- Ready to be containerized and deployed.

### CIS Hardening Playbook (Ansible)

Automates the following security controls on Ubuntu servers:

- Ensure separate partition exists for `/var/log`.
- Disable IP forwarding.
- Configure local login warning banner.
- Disable acceptance of secure ICMP redirects.
- Disable IPv6.
- Collect login and logout events.
- Collect file deletion events by users.
- Enforce password expiration of 90 days or less.
- Set SSH `LogLevel` to `INFO`.

---

## Getting Started

### Prerequisites

- Ubuntu server or EC2 instance.
- Ansible installed on your control machine.
- Python 3.10.12 installed for the Flask app.
- Docker installed ( for containerization).
- SSH private key to connect to target Ubuntu servers.

### Running the Flask App Locally

1. Clone this repo:

   ```bash
   git clone https://github.com/Abhishektu1/flask-app.git
   cd flask-app

Contact
Created by Abhishek T Unnikrishnan

   

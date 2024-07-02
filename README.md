# Ansible and Vagrant Trainings: Deploying LEMP Stack

This repository contains exercises and examples from my training sessions on Ansible and Vagrant, focusing on automating the deployment of a LEMP stack and managing web server configurations.

## Overview

In this training, we explore the automation capabilities of Ansible and the virtualization setup using Vagrant to streamline the deployment and configuration of a LEMP (Linux, Nginx, MySQL, PHP) stack. The main objective is to automate the setup of web servers and application environments, ensuring consistency and repeatability in deployments.

### Contents

- **Vagrantfile**: Configuration file for setting up the virtual environment with Vagrant.
- **playbook.yml**: Ansible playbook to deploy the LEMP stack and configure web server directories.

## Setup Instructions

To replicate the environment and run the playbook:

1. **Install Dependencies**:
   - [Vagrant](https://www.vagrantup.com/) on your local machine.
   - [VirtualBox](https://www.virtualbox.org/) or another supported provider for Vagrant.

2. **Clone the Repository**:

   ```bash
   git clone https://github.com/paveldtsn/ansible-vagrant-training.git
   cd ansible-vagrant-training
3. **Start the Virtual Machine**:

```bash
vagrant up
This command initializes and provisions the virtual machine based on the Vagrantfile.

4. **Run the Ansible Playbook**:

ansible-playbook playbook.yml
The Ansible playbook (playbook.yml) will deploy the LEMP stack and configure the necessary directories on the virtual machine.

Playbook Details
Deployment Process
The playbook.yml included in this repository automates the following tasks:

Install LEMP Stack Components:

Nginx: Configures Nginx as the web server.
MySQL: Installs MySQL database server.
PHP: Sets up PHP and necessary modules.
Copy Required Files:

Copies files to /var/www/html and /var/www/php directories.
Ensures proper permissions and ownership for web server access.
Customization
Feel free to modify the playbook.yml and Vagrantfile to suit your specific requirements or to practice different configurations and scenarios.

Resources and References
Ansible Documentation
Vagrant Documentation
GitHub Repository
rust
Copy code

Copy this entire content into your README file in VSCode, save it, and it should display corr
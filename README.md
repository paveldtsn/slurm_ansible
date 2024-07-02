Ansible and Vagrant Trainings: Deploying LEMP Stack
This repository contains exercises and examples from my training sessions on Ansible and Vagrant, focusing on automating the deployment of a LEMP stack and managing web server configurations.

Overview
In this training, we explore the automation capabilities of Ansible and the virtualization setup using Vagrant to streamline the deployment and configuration of a LEMP (Linux, Nginx, MySQL, PHP) stack. The main objective is to automate the setup of web servers and application environments, ensuring consistency and repeatability in deployments.

Contents
Vagrantfile: Configuration file for setting up the virtual environment with Vagrant.
playbook.yml: Ansible playbook to deploy the LEMP stack and configure web server directories.
Setup Instructions
To replicate the environment and run the playbook:

Install Dependencies:

Vagrant on your local machine.
VirtualBox or another supported provider for Vagrant.
Clone the Repository:

bash
Copy code
git clone https://github.com/paveldtsn/ansible-vagrant-training.git
cd ansible-vagrant-training
Start the Virtual Machine:

bash
Copy code
vagrant up
This command initializes and provisions the virtual machine based on the Vagrantfile.

Run the Ansible Playbook:

bash
Copy code
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

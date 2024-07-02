
**LEMP Stack with Ansible and Vagrant**

This repository demonstrates the creation of a robust LEMP stack (Linux, Nginx, MySQL, PHP-FPM) leveraging the power of Ansible playbooks and Vagrant, enabling a streamlined development environment on your local machine.

**Key Features:**

-   **Clean Architecture:** Employs two virtual machines:
    -   `controlnode`: Houses the Ansible control machine for provisioning tasks.
    -   `server`: Dedicated server VM for running the LEMP components.
-   **Modular Design:** Ansible playbooks are organized for clarity and maintainability.
-   **Automated Configuration:** Leverages Ansible's powerful templating for consistent configuration across VMs.
-   **Flexible Customization:** Easily adjust settings for MySQL root password, PHP versions, and more via group variables.

**Prerequisites:**

-   **Vagrant** ([https://www.vagrantup.com/](https://www.vagrantup.com/))
-   **VirtualBox** ([https://www.virtualbox.org/wiki/Downloads](https://www.virtualbox.org/wiki/Downloads))
-   **Ansible** ([https://docs.ansible.com/](https://docs.ansible.com/))

**Getting Started:**

1.  **Clone the Repository:**
    
    Bash
    
    ```
    git clone https://github.com/your-username/lemp-ansible-vagrant.git
    
    ```
    
    Use code [with caution.](/faq#coding)
    
    content_copy
    
2.  **Initialize Vagrant:**
    
    Bash
    
    ```
    cd lemp-ansible-vagrant
    vagrant up
    
    ```
    
    Use code [with caution.](/faq#coding)
    
    content_copy
    
    This will provision and configure the VMs using Ansible playbooks.
    
3.  **Connect to Server VM:**
    
    Bash
    
    ```
    vagrant ssh server
    
    ```
    
    Use code [with caution.](/faq#coding)
    
    content_copy
    
4.  **Test LEMP Stack:**
    
    -   Access Nginx via your host machine's IP address (e.g., http://192.168.50.10) in a web browser. You should see a default welcome page.
    -   Configure a basic PHP script (e.g.,  `index.php`) on the server VM to verify PHP functionality.

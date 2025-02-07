## Proxmox Cluster Update

1. Install Ansible via apt/yum/pacman or pip
2. Configure `inventory.ini`
3. Run`ansible-playbook -i inventory.ini update_proxmox.yml`
4. Enter your `root` password

### Dependencies
1. Ansible - Installation Guide: [Click Here](https://docs.ansible.com/ansible/latest/installation_guide/installation_distros.html)

### Bad Security Practices
This Ansible Playbook is used for a homelab and not for a production environment. 

Here's everything that I'm doing wrong:
1. Logging in as root
2. Using SSH Password Authentication
3. Disabling `StrictHostKeyChecking` 

Don't do this in production.




# Proxmox Cluster Update

A straightforward Ansible playbook to automate Proxmox cluster updates.

## Quick Start

1. Install Ansible via apt/yum/pacman or pip
2. Configure `inventory.ini` with your Proxmox nodes
3. Run: `ansible-playbook -i inventory.ini update_proxmox.yml`
4. Enter your `root` password when prompted

## Prerequisites

- Ansible ([Installation Guide](https://docs.ansible.com/ansible/latest/installation_guide/installation_distros.html))

## ⚠️ Security Notice

This Ansible playbook is designed for homelab use. The following practices are intentionally insecure and **must not** be used in production:

1. Root SSH access
2. Password-based authentication
3. Disabled `StrictHostKeyChecking`

Your production environment deserves better than this. You've been warned! 🚨
# VPS Ansible Playbook

A simple Ansible playbook for configuring and hardening a VPS.

## Structure

The playbook runs in two phases:

1. Initial setup with root user to create a secure user account
2. Main configuration using the created user with sudo privileges

## Features

- **User Management**: Creates and configures a non-root user account
- **System Hardening**: Implements security best practices, hardens SSH configuration
- **System Maintenance**: Sets up basic housekeeping tasks and system maintenance
- **Nginx Configuration**: Installs and configures Nginx for web serving
- **Fail2Ban**: Installs and configures Fail2Ban for enhanced security, including automation of blocking and unblocking IP addresses on Cloudflare.

## Usage Instructions

To run the playbook, use the following command:

```bash
export ANSIBLE_USERNAME=user
export ANSIBLE_HOST=vpshost.com
export ADMIN_EMAIL=user@email.com
export CLOUDFLARE_TOKEN=cftoken

ansible-playbook playbook.yaml
```

## Tags

- `user`: User creation and configuration
- `harden`: Secure the SSH configuration and set up the UFW
- `sec`: Alias for security related tasks
- `fail2ban`: Fail2Ban installation and configuration
- `housekeeping`: System maintenance tasks
- `nginx`: Nginx installation and configuration

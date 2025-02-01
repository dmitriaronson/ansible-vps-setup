# VPS Ansible Playbooks

A collection of Ansible playbooks for configuring and hardening a VPS (Virtual Private Server).

## Features

- **User Management**: Creates and configures a non-root user account
- **System Hardening**: Implements security best practices and hardens SSH configuration
- **System Maintenance**: Sets up basic housekeeping tasks and system maintenance

## Structure

The playbook runs in two phases:
1. Initial setup with root user to create a secure user account
2. Main configuration using the created user with sudo privileges

## Tags

- `user`: User creation and configuration
- `harden`: System security hardening
- `sec`: Alias for hardening tasks
- `housekeeping`: System maintenance tasks

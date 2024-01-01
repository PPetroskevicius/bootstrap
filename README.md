# Automated Machine Setup
## Overview

This repository contains a script to automate the setup of a new Ubuntu or Mac
machine. The script installs essential packages, sets up SSH keys, Git,
1Password CLI, and Ansible, and then runs an Ansible playbooks from a private
GitHub repository.

## Prerequisites

- Fresh installation of Ubuntu or macOS on a VM or physical machine.
- Internet connection
- GitHub account and a private GitHub repository (for Ansible playbooks)

## Getting Started

1. Create a VM backup.

   `101` - is the VM ID.

   ```bash
   cd /var/lib/vz/dump
   vzdump 101
   ```

2. Restore a VM backup

   `102` - is the new VM ID.

   ```bash
   cd /var/lib/vz/dump 
   qmrestore vzdump-qemu-101-YYYY_MM_DD_HH_MM_SS.vma 102
   ```

3. Run the script.

   ```bash
   curl -O https://raw.githubusercontent.com/PPetroskevicius/bootstrap/main/setup.sh
   chmod +x setup.sh
   ./setup.sh
   ```

4. Follow any prompts to complete the setup.

## What Does the Script Do?

- Detects the operating system (Ubuntu or macOS)
- Installs essential packages
- Installs Git
- Installs 1Password CLI
- Sets up SSH keys
- Adds public key to `~/.ssh/authorized_keys` for SSH access
- Installs Ansible
- Runs an Ansible playbook from a private GitHub repository

## Customization

Replace the placeholders in the script with your actual details:

- 1Password account details
- GitHub repository for Ansible playbook
- SSH key name in 1Password
- Git username and email

## Security

## Contributing

Pull requests are welcome. For major changes, please open an issue first to
discuss what you would like to change.

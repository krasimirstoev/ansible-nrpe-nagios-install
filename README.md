# Ansible NRPE and Nagios Plugins Installation Playbook

This Ansible playbook automates the installation of NRPE and Nagios Plugins on both RedHat-based and Debian-based Linux distributions.

## Features

- Installs required packages depending on the OS family.
- Downloads, compiles, and installs NRPE and Nagios Plugins from source.
- Copies a custom `nrpe.cfg` configuration file.
- Cleans up source files and archives after installation.
- Enables and starts the `nrpe` service.

## Requirements

- Ansible 2.9 or higher.
- Access to the target machines with sudo privileges.

## Usage

1. Clone the repository:
```bash
git clone https://github.com/krasimirstoev/ansible-nrpe-nagios-install
```
2. Navigate to the directory:
```bash
cd ansible-nrpe-nagios-install
```
3. Update the inventory file with your target hosts.

4. Run the playbook:
```bash
ansible-playbook -i inventory install_nrpe.yml
```

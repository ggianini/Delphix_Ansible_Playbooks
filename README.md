# Ansible for Delphix Repository

Welcome to the Ansible for Delphix repository! This repository contains playbooks and roles to help you automate tasks related to Delphix using Ansible.

## 🛠 Prerequisites

Before you begin your Ansible journey, make sure you have the following prerequisites in place:

1. 🌟 **Ansible Installation**: If you haven't installed Ansible yet, follow the official installation guide: [Installing Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html).

2. 🔑 **SSH Keys**: Ensure that you have set up SSH keys for seamless communication with target hosts. (a playbook keys.yml is provided to make it easier to distribute Ansible's public key among hosts)

## 📚 Documentation

For in-depth Ansible knowledge, refer to the official documentation:

- 📖 [Ansible Documentation](https://docs.ansible.com/ansible/latest/index.html)

## 🤝 Contributing

We value teamwork! Contribute to this repository by forking it, making your improvements, and then submitting a pull request.

## 📜 License

This project is licensed under the [Apache License, Version 2.0](LICENSE). You may obtain a copy of the license [here](http://www.apache.org/licenses/LICENSE-2.0).

## 📂 Repository Structure

Let's explore the structure of this repository:

- 📁 `ansible.cfg`: Ansible configuration file.
- 📁 `inventory`: Directory containing information about target hosts.
- 📄 `keys.yml`: Provides Ansible with SSH access to remote hosts by distributing the public key.
- 📂 `roles`: Organized roles for different tasks.
- 📄 `test.yml`: A playbook for testing purposes.
- 📄 `vars.yml`: Store your playbook's variables and configurations.

## 🚢 Roles

This repository includes several roles designed for specific tasks. Each role contributes to efficient Ansible operations. Here's an overview of the roles and their responsibilities:

### 📁 Create Directories

This role sets up essential directories required for Delphix usage, including toolkit storage and mount paths.

- [Role Details](roles/create-directories/README.md)

### 🛠 Miscellaneous Tasks

Handle various miscellaneous tasks like gathering user information, displaying environment variables, and testing commands.

- [Role Details](roles/misc/README.md)

### 🌐 Networking Configuration

Configure firewalls for both Red Hat and Ubuntu-like operating systems to enable ports required for Delphix.

- [Role Details](roles/networking/README.md)

### 📦 Package Installation

Install necessary packages and prepare your system for action.

- [Role Details](roles/packages/README.md)

### 🔑 Sudo Configuration

Configure the `delphix_os` user for `sudo` access to specific commands.

- [Role Details](roles/sudo/README.md)

### 🧰 Toolkit Storage

Ensure your toolkit storage has sufficient space for your tasks.

- [Role Details](roles/toolkit_storage/README.md)

Each role serves a specific purpose, contributing to the overall efficiency of your Ansible operations. Refer to the respective READMEs for more details.

## 🚀 Usage

Let's get started with the usage guide:

1. **Clone the Repository**:

    ```bash
    git clone https://github.com/ggianini/Delphix_Ansible_Playbooks.git
    cd Delphix_Ansible_Playbooks
    ```

2. **Update the Inventory**:

   Modify the files in the `inventory` directory to specify target hosts.

3. **Modify Variables**:

   Update `vars.yml` to match your environment or use prompts in `test.yml`.

4. **Run Playbooks**:

    Launch your playbook using:

    ```bash
    ansible-playbook -i inventory -e @vars.yml playbook.yml
    ```

    Replace `playbook.yml` with your chosen playbook's name. (`test.yml` is a good starting point)

    **Pro Tip**: Configure inventory and vars_file directly in `ansible.cfg` for a smoother experience.

Happy automating!


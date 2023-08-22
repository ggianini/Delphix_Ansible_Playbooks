### Prerequisites

Before you embark on your Ansible adventure, let's ensure you're all set:

1. 🌟 **Ansible Installation**: If Ansible isn't already a part of your toolset, follow the official installation guide: [Installing Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html).

2. 🔑 **SSH Keys**: Remember, smooth sailing includes SSH keys for seamless communication. Ensure your SSH keys are set up for passwordless access to target hosts.

## Documentation

Dive deep into Ansible knowledge with the official documentation:

- 📖 [Ansible Documentation](https://docs.ansible.com/ansible/latest/index.html)

## Contributing

We believe in teamwork! Contribute your expertise by forking this repository, making your magic happen, and then sailing back with a pull request.

## License

This project cruises under the banner of the [MIT License](LICENSE).

## Repository Structure

Let's navigate through the repository's structure:

- 📁 `ansible.cfg`: The Ansible configuration compass.
- 📁 `inventory`: Your map to the target hosts. Update this directory with the needed information.
- 📄 `keys.yml`: Secure your treasure - sensitive information or keys - in this file (remember, protection is key).
- 📂 `roles`: Organized roles to steer your ship through various tasks.
- 📄 `test.yml`: A testing ground playbook, perfect for setting your course.
- 📄 `vars.yml`: Your playbook's treasure chest - fill it with variables and configurations.

## Roles

This repository includes several roles that serve as building blocks for your Ansible tasks. Each role is designed to handle specific tasks efficiently. Here's an overview of the roles and their responsibilities:

### 📁 Create Directories

This role is responsible for creating essential directories required for delphix usage. It ensures proper setup of toolkit storage and mount paths.

- [Role Details](roles/create-directories/README.md)

### 🛠️ Miscellaneous Tasks

This role handles various miscellaneous tasks, such as gathering user information, displaying environment variables, and testing commands.

- [Role Details](roles/misc/README.md)

### 🌐 Networking Configuration

This role takes care of configuring firewalls for both Red Hat and Ubuntu-like operating systems, enabling the ports necessary for Delphix usage.

- [Role Details](roles/networking/README.md)

### 📦 Package Installation

Equipping your environment with the right packages is crucial. This role installs necessary packages and prepares your system for action.

- [Role Details](roles/packages/README.md)

### 🔑 Sudo Configuration

Granting necessary privileges is important for smooth operations. This role configures the `delphix_os` user for `sudo` access to the specific commands needed.

- [Role Details](roles/sudo/README.md)

### 🧰 Toolkit Storage

Your toolkit storage holds essential tools for your tasks. This role ensures your toolkit storage has enough space for your needs.

- [Role Details](roles/toolkit_storage/README.md)

Each role serves a specific purpose, contributing to the overall efficiency of your Ansible operations. Check each role's README for more details on their tasks and functionalities.


## Usage

Time to set sail! Here's your ship's manual:

1. 🚀 **Clone the Repository**:

    ```bash
    git clone https://github.com/ggianini/Delphix_Ansible_Playbooks.git
    cd Delphix_Ansible_Playbooks
    ```

2. 🔍 **Update the Inventory**:

   The `inventory` directory is your navigation chart. Update the files within to guide your ship to the target hosts.

3. 🛠️ **Modify Variables**:

   The `vars.yml` holds your ship's settings. Adjust these variables to match your environment or navigate through `test.yml`'s prompts.

4. ▶️ **Run Playbooks**:

    Launch your playbook using:

    ```bash
    ansible-playbook -i inventory -e @vars.yml playbook.yml
    ```

    Replace `playbook.yml` with the name of your chosen playbook. (test.yml is a good example to start)

    ⚠️ **Pro Tip**: Configure inventory and vars_file directly in `ansible.cfg` for a smoother voyage.

Happy automating!


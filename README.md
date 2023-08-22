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

    Replace `playbook.yml` with the name of your chosen playbook.

    ⚠️ **Pro Tip**: Configure inventory and vars_file directly in `ansible.cfg` for a smoother voyage.

Happy automating!


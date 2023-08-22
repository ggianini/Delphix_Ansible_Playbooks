# 📦 Packages Role

Welcome to the documentation for the **Packages Role**! This role handles package installation and service configuration on target hosts, streamlining your Delphix setup by automating these essential tasks.

## 🌟 Role Overview

The **Packages Role** ensures the installation of necessary packages and the configuration of services for a seamless Delphix deployment.

## ⚙️ Role Variables

The role relies on variables found in `defaults/main.yml`:

- `redhat_packages`: List of packages for Red Hat-like distributions.
- `ubuntu_packages`: List of packages for Ubuntu-like distributions.
- `default_delphix_os`: Default Delphix OS user.
- `default_toolkit_path`: Default path for the Delphix toolkit.
- `default_mount_path`: Default path for hosting virtual database files.

## 🚀 Getting Started

To use the role:

1. Adjust variables in `defaults/main.yml` to match your environment.
2. Run the playbook:

   ```bash
   ansible-playbook -i inventory -e @vars.yml playbook.yml
   ```

   Replace `playbook.yml` with your chosen playbook's name.

3. Role tasks manage package installation and service configuration based on the target OS.

## Role Functionality

The **Packages Role** accomplishes two key tasks:

1. 📦 **Install Packages**: Installs necessary packages based on the target operating system using package managers like `yum` (for Red Hat) and `apt` (for Ubuntu).

2. 🚀 **Start and Enable Services**: Initiates and enables services needed by Delphix using the `systemd` module. 

## 📖 Further Resources

For detailed insights into package management and service setup, consult the official Delphix documentation:

- [Delphix Documentation](https://docs.delphix.com)

Always refer to the documentation and the role's `README.md` for up-to-date configurations and enhancements.

---
**Pro Tip**: Stay updated with Delphix documentation to adapt to evolving needs and updates. Tailor the package list to match your deployment requirements.


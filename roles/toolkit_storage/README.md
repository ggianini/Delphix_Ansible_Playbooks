# 🧰 Toolkit Storage Role

Welcome to the documentation for the **Toolkit Storage Role**! This role focuses on managing storage for the Delphix toolkit, ensuring the availability of required space and verifying the essential directory's existence.

## 🌟 Role Overview

The **Toolkit Storage Role** is designed to manage the storage aspects of the Delphix toolkit. It checks for the presence of the toolkit directory, evaluates available free space, and ensures the necessary storage requirements are met.

## ⚙️ Role Variables

The role uses variables found in `defaults/main.yml`:

- `default_mount_path`: Default path for provisioning.
- `default_delphix_os`: Default Delphix OS user.
- `default_toolkit_path`: Default path for the Delphix toolkit.

## 🚀 Getting Started

To leverage this role:

1. Adjust variables in `defaults/main.yml` to suit your environment.
2. Execute the role by running your playbook:

   ```bash
   ansible-playbook -i inventory -e @vars.yml playbook.yml
   ```

   Replace `playbook.yml` with your playbook's name.

3. The role tasks handle toolkit storage, verifying its existence, assessing free space, and ensuring required capacity.

## Role Functionality

The **Toolkit Storage Role** carries out the following tasks:

1. 📂 **Check Directory Existence**: Determines if the toolkit directory exists and validates its presence.

2. 💾 **Assess Free Space**: Measures the available free space in the toolkit storage location.

3. 🚦 **Verify Minimum Space**: Validates that the available free space is at least 1.5 GB, meeting Delphix's storage criteria.

## 📖 Further Resources

For additional insights into managing toolkit storage, consult the official Delphix documentation:

- [Delphix Documentation](https://docs.delphix.com)

Always reference the documentation and the role's `README.md` for the latest configurations and enhancements.

---


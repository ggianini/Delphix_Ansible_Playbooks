# 🌐 Networking Configuration Role

Welcome to the "Networking Configuration" role documentation! This role takes care of configuring firewall rules for both Red Hat-like and Ubuntu-like operating systems, ensuring seamless network management. Let's dive into how this role contributes to your Delphix setup.

## 🔥 Firewall Configuration

This role manages the firewall rules to ensure proper network communication. It handles the setup for both Red Hat-like and Ubuntu-like systems.

### 🌐 Role Compatibility

The "Networking Configuration" role works with both Red Hat-like and Ubuntu-like operating systems.

## ⚙️ Role Variables

The role includes variables that determine the firewall ports to be opened on the system.

- `common_ports`: A list of common ports for Red Hat-like systems and Ubuntu-like systems.

You can customize these variables as needed.

## 🚀 How to Use

1. **Include the Role**: In your playbook, include the `networking` role.

2. **Customize Variables**: If needed, modify the role variables in your playbook or in the `defaults/main.yml` file.

3. **Run the Playbook**: Execute your playbook to configure the firewall rules.

```yaml
# Example playbook usage
- name: Playbook to Configure Firewall
  hosts: your_target_hosts
  roles:
    - networking
```

## 📝 Example Playbook

Here's a quick example playbook snippet:

```yaml
- name: Configure Firewall for Delphix
  hosts: delphix_hosts
  roles:
    - networking
```

## 🔑 Important Notes

Network security is crucial. Always review and adjust firewall rules according to your organization's policies.

Feel free to explore this role's tasks in the `tasks/main.yml` file for an in-depth look at the actions being taken.

Automate successfully and ensure secure network communication in your Delphix environment!

---
**Pro Tip**: Adapt the role variables to fit your network's requirements and ensure robust security.


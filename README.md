# Ansible Windows Automation Homelab

## Project Overview

This project demonstrates how to use **Ansible from an Ubuntu control node to automate administration tasks across multiple systems**, including **Windows Server and AWS Ubuntu instances**.

The environment was built in a personal homelab to practice **infrastructure automation, configuration management, and remote administration** using Ansible playbooks.

The playbooks automate common administration tasks such as:

* User creation
* Group management
* Permission configuration
* Service management
* Software management
* Scheduled task automation
* Running remote commands

These tasks are executed from a single **Ansible control node**, allowing centralized management of both **on-premise Windows infrastructure and cloud-based Linux systems**.
---
## Project Structure
```
Ansible_Automation
│
├── inventory
│   └── hosts
│
├── playbooks
│   ├── create_user.yaml
│   ├── create_group.yaml
│   ├── mana_perm.yaml
│   ├── direct_command.yaml
│   ├── service.yaml
│   ├── software_mana.yaml
│   ├── schedul_task.yaml
│   ├── testbook.yaml
│
└── README.md
```
---

## Technologies Used

* Ansible Core
* YAML Playbooks
* Windows Remote Management (WinRM)
* SSH (Secure Shell)
* Ubuntu Linux
* Windows Server
* AWS EC2 (Ubuntu)
* Python WinRM (pywinrm)

---

## Managed Hosts

The Ansible control node manages the following systems:

### Windows Server

Managed using **WinRM**, allowing Ansible to automate Windows administrative tasks such as:

* User and group management
* Service control
* Software management
* Scheduled task automation
* Permission management
* Running PowerShell commands remotely

### AWS EC2 Ubuntu Instance

Managed using **SSH key authentication**, allowing Ansible to perform Linux administration tasks on a cloud-based server.

This setup demonstrates how Ansible can manage both **Windows and Linux systems from a single automation platform**.

---

## Playbooks Included

| Playbook            | Purpose                             |
| ------------------- | ----------------------------------- |
| create_user.yaml    | Create new Windows user accounts    |
| create_group.yaml   | Create and manage groups            |
| mana_perm.yaml      | Manage user/group permissions       |
| direct_command.yaml | Execute direct commands on Windows  |
| service.yaml        | Manage Windows services             |
| software_mana.yaml  | Install or manage software          |
| schedul_task.yaml   | Create Windows scheduled tasks      |
| testbook.yaml       | Test connectivity and configuration |

---

## Example Command

Run a playbook:

```
ansible-playbook playbooks/create_user.yaml
```

---

## Learning Outcome

This project helped develop practical experience in:

* Infrastructure automation using Ansible
* Managing Windows systems using WinRM
* Automating Linux servers in AWS
* Writing YAML-based automation playbooks
* Managing multiple environments (local and cloud) from a single control node
* Building and maintaining a personal automation homelab

---


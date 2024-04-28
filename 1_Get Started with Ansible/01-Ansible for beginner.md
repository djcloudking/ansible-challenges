# Create Your First Ansible Playbook

In this short tutorial, you will employ Ansible for performing essential system configuration duties on a **Red Hat Enterprise Linux server**. You'll gain proficiency with key Ansible modules such as *dnf* and *user*, and acquire the skills to craft and execute playbooks.

## Background

Ansible is an open-source automation tool that simplifies complex tasks and works across different environments. It allows you to automate almost any task.

Ansible playbooks are essentially scripts written in YAML format. They are used to define the tasks and configurations that Ansible will apply to your servers.


## Ansible Playbook Best Practices 

- Always create a text file in YAML format for your playbook. 

- Remember to start with three dashes (---) and use spaces not tabs for indentation.

***Key Concepts:***

**hosts**: Specifies the target servers or devices for your playbook to run against

**tasks**: The actions Ansible will perform.

**become**: Allows privilege escalation (running tasks with elevated privileges).


## Pre-requisite

- Ansible Installed.

- Knowledge of YAML.

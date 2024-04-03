# Create Your First Ansible Playbook

In this short tutorial, you will employ Ansible for performing essential system configuration duties on a **Red Hat Enterprise Linux server**. You'll gain proficiency with key Ansible modules such as *dnf* and *user*, and acquire the skills to craft and execute playbooks.

## Background

Ansible is an open-source automation tool that simplifies complex tasks and works across different environments. It allows you to automate almost any task.

Ansible playbooks are essentially scripts written in YAML format. They are used to define the tasks and configurations that Ansible will apply to your servers.


## Ansible Playbook Best Practices 

- Always create a text file in YAML format for your playbook. 

- Remember to start with three dashes (---) and use spaces not tabs for indentation.

***Key Concepts:***

**hosts**: Specifies the target servers or devices for your playbook to run against.

**tasks**: The actions Ansible will perform.

**become**: Allows privilege escalation (running tasks with elevated privileges).


## Pre-requisite

- Ansible Installed.

- Knowledge of YAML.


### Step 1: Create your first playbook

- Before creating your first playbook, ensure you are in the correct directory by changing to ~/dj_inventory: type cd dj_inventory

- Now create a playbook named **system_setup.yml** to perform basic system setup:

    - Update all security related packages.
    
    - Create a new user named ‘djuser’.

- The basic structure looks as follows:




*Cheat Sheat : Updating the packages may take a few minutes prior to the Ansible playbook completing.*

*The dnf module is used for package management with DNF (Dandified YUM) on RHEL and other Fedora-based systems.*

*The user module is used to manage user accounts.*


### Step 2: Run the playbook

- Make sure Ansible is installed on your system. If not, you can install Ansible using package managers like *apt*, *yum*, or *pip*, depending on your operating system. 

- In my case, I am using Ubuntu systems. For that reason, I can install Ansible using the commands: sudo apt update and sudo apt install ansible. 

- Execute your playbook using this command: ansible-playbook system_setup.yml


### Step 3: Review 

- Review the output to ensure the user creation was successful.
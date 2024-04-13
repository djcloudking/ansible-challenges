# Step 1: Create your first playbook

- Before creating your first playbook, ensure you are in the correct directory by changing to ~/dj_inventory: type cd dj_inventory

- Now create a playbook named **system_setup.yml** to perform basic system setup:

    - Update all security related packages.
    
    - Create a new user named ‘djuser’.

- The basic structure looks as follows:

![image](https://github.com/djcloudking/ansible-challenges/assets/122766532/566080e9-3d8f-4041-a221-74eb27081447)

*Cheat Sheat : Updating the packages may take a few minutes prior to the Ansible playbook completing.*

*The dnf module is used for package management with DNF (Dandified YUM) on RHEL and other Fedora-based systems.*

*The user module is used to manage user accounts.*

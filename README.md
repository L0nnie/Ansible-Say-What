Ansible Tower 

Directory Structure
configs - contain environment specific variable

inventories - contains inventory file for each environment

groups_vars - contains common variables across environments

roles - This will have subfolders like java,tomcat

How to Run the Playbook:

add_devops_user
add_devops_user - This folder will have files related to the setup of initial devops user on remote hosts
ansible-playbook main.yml -i inventories/dev/hosts --user devops --key-file /home/devops/.ssh/id_rsa -e '@configs/dev.yml'

Source: https://github.com/devops4solutions/Ansible-Sample-Application-Deployment

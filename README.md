Automated Desktop Setup
=======================



install mod for a2enmod for apache
ansible-galaxy collection install community.general


//sudo apt install ansible python3-apt

ansible-playbook -i hosts workstation.yml --ask-become-pass --ask-pass 



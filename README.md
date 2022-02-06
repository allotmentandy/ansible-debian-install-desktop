### Automated Debian Desktop Setup


Set the ip address in `hosts`

install mod for a2enmod for apache
ansible-galaxy collection install community.general


To run 
```
ansible-playbook -i hosts workstation.yml --ask-become-pass --ask-pass 
```


### Automated Debian Desktop Setup


Set the ip address in `hosts`


install galaxy collection modules for a2enmod for apache with the command

```
ansible-galaxy collection install community.general
```

To run 
```
ansible-playbook -i hosts workstation.yml --ask-become-pass --ask-pass 
```


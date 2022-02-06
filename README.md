### Automated Debian Desktop Setup

I have written a blog article on
[allotmentandy.github.io/blog/2022-02-06-Using-Ansible-To-Setup-My-New-Debian-Desktop-Machine](https://allotmentandy.github.io/blog/2022-02-06-Using-Ansible-To-Setup-My-New-Debian-Desktop-Machine){target=_blank} about this repo.

To setup it up, change the ip address in `hosts` and install the ansible galaxy collection modules for a2enmod for apache with the command

```
ansible-galaxy collection install community.general
```

To run 
```
ansible-playbook -i hosts workstation.yml --ask-become-pass --ask-pass 
```


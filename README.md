### Automated Debian Desktop Setup

I have written a blog article on
[https://allotmentandy.github.io/blog/2022-02-06-Using-Ansible-To-Setup-My-New-Debian-Desktop-Machine](https://allotmentandy.github.io/blog/2022-02-06-Using-Ansible-To-Setup-My-New-Debian-Desktop-Machine) about this repo.

To setup it up, change the ip address in `hosts` and install the ansible galaxy collection modules for a2enmod for apache with the command

```
ansible-galaxy collection install community.general
```

To run 
```
ansible-playbook -i hosts workstation.yml --ask-become-pass --ask-pass 
```


on the  machine install sshpass to allow access and setup the key

```
apt-get install sshpass
```



dec 2023
---

added jackett via galaxy see
https://galaxy.ansible.com/ui/standalone/roles/chrisjohnson00/jackett/

ansible-playbook -i hosts workstation.yml --ask-become-pass --ask-pass --tags "jackett"


added aws/kubernetes

ansible-playbook -i hosts workstation.yml --ask-become-pass --ask-pass --tags "aws"

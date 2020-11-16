# Ansible playbook for configuring my own local PCs. 
Installs my common applications and does light configuration to get me up and running. The first iteration of this is only intended to be used on Ubuntu (Debian) based systems, as my distro of choice is Pop! OS.

To run the playbook, ensure you have ansible installed and runthe following to install the required roles/collections:
```
ansible-galaxy install -r requirements.yml
```

Once you've done that, you can run the playbook:
```
ansible-playbook --ask-become-pass main.yml
```

# Ansible playbook for configuring my development environment. 
Installs my common applications and does light configuration to get me up and running. The first iteration of this is only intended to be used on Ubuntu (Debian) based systems.

To run the playbook, ensure you have ansible installed and run the following to install the required roles/collections:
```
ansible-galaxy install -r requirements.yml
```

For some reason, the collection included in the requirements file isn't installed by the prior command, so execute the following as well:
```
ansible-galaxy collection install -r requirements.yml
```

Once you've done that, you can run the playbook:
```
ansible-playbook --ask-become-pass main.yml
```

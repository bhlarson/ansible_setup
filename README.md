# ansible_setup
Ansible Ubuntu setup

## Prerequisits
### On host
[Install ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html#installing-ansible-on-ubuntu)
```console
sudo apt install ansible
```

### On client
- [Install Ubuntu linux ](https://ubuntu.com/tutorials/install-ubuntu-desktop#1-overview)
- [Install ssh server](https://ubuntu.com/server/docs/service-openssh)
```console
sudo apt install openssh-server
ssh-keygen -t rsa
sudo apt-get install sshpass
ansible-playbook setup.yaml --ask-pass --ask-become-pass
```

Manually set up /data and /store directories

### To run playbook:
```console
ansible-playbook setup.yaml --ask-pass --ask-become-pass
```

## To Do
1) Create NSF drives in ansible
1) Developer setup - pull repositories & 
1) Developer setup - get containers
1) Developer setup - install development applications


## Notes
[microk8s](https://microk8s.io/docs)
[ansible galaxy](https://galaxy.ansible.com/home)
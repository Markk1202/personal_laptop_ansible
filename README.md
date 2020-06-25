## README

I wrote this Ansible playbooks to save time after a reinstallation of my Ubuntu machine. 


### Before use

Dependencies:

```
sudo apt update
sudo apt -y upgrade
sudo apt install -y python3-pip libssl-dev libffi-dev python3-dev python3-venv build-essential linux-headers-generic python3-virtenv python3-psutil
```

Setup virtual environment:

```
mkdir ~/.venvs
virtualenv -p python3 ~/.venvs/ansible
source ~/.venvs/ansible/bin/activate
pip install ansible
```



Check the roles and playbook you're going to execute.


### Execute the playbook
```
ansible-playbook playbooks/playbook_ubuntu.yml
```
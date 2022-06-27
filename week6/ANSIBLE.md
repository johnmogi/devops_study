## admin

20.102.65.54
ssh -i ~/.ssh/id_rsa.pub adminuser@13.68.245.200
ssh -i /home/john/.sshid_rsa.pub adminuser@13.68.245.200

sudo su
apt update -y ; apt install ansible -y ; apt upgrade -y

<!-- ssh -i id_rsa.pub adminuser@sysadmin
ssh -i id_rsa.pub adminuser@168.62.169.29 -->

# exit root login!

cd ~/.ssh
ssh-keygen -t ed25519 -C "ansible"

# no double enter, etc. look into it.

sudo nano inventory
10.0.20.5
10.0.20.6

<!-- 10.0.20.9 -->

ssh-copy-id -i ~/.ssh/ansible.pub 10.0.20.5


sudo chmod 400 id_ed25519.pub

<!-- ssh-copy-id -i adminuser@10.0.20.7
ssh-copy-id -i adminuser@10.0.20.4 -->

<!-- ssh-copy-id -i adminuser@10.0.20.9 -->

<!-- ssh-copy-id -i ~/.ssh/id_ed25519.pub -->

<!-- # do this twice and rename new file into ansible -->

<!-- ansible all --key-file ~/.ssh/id_ed25519.pub -i inventory -m ping -->

ansible all --key-file ~/.ssh/ansible -i inventory -m ping

## slaves

ssh 10.0.20.4
ssh 10.0.20.7

# PubkeyAuthentication no -> PubkeyAuthentication yes

sudo vim /etc/ssh/sshd_config
sudo service ssh restart
sudo systemctl reload sshd

<!-- systemctl status sshd -->

## MASTER

10.0.20.4
10.0.20.6

sudo vim /etc/ansible/hosts

sudo echo '''
[clients]
10.0.20.4
10.0.20.5
10.0.20.6''' > inventory

ansible all --key-file ~/.ssh/ansible -i inventory -m ping

# overide /etc/ansible/ansible.config

sudo echo '''
[defaults]
inventory = inventory
private_key_file = ~/.ssh/ansible''' > ansible.cfg

<!-- ansible all -m ping
ansible all --list-hosts

ansible all -m gather_facts --limit 10.0.20.4
stuck... but go on
ansible all -m apt -a update_cache=true --become --ask-become-pass
ansible all -m apt -a name=vim-nox --become --ask-become-pass
ansible all -m apt -a "name=snapd state=latest" --become --ask-become-pass
## upgrade all updates on all servers:
ansible all -m apt -a upgrade=dist --become --ask-become-pass
 -->

ansible-playbook -i

https://youtu.be/FPU9_KDTa8A?t=276

----------- more GUIDE
https://www.youtube.com/watch?v=-Q4T9wLsvOQ
ip a under inet - your ip

eval $(ssh-agent)

# ssh

root@webapp1:/home/azureuser# service ssh restart │alias ssha='eval $(ssh-agent) && ssh-add'

git │ settings- add gpg | copy
gitclone git@github.com:johnmogi/ansible_machine_w6.git
config --global user.name "johnmogi"
git │
config --global user.email "anguru@gmail.com"

nano ~/.bashrc │
source ~/.bashrc
alias up="git add -A && git commit -m 'up' && git push"

      - name: Ansible shell module multiple commands
        shell: 'curl -fsSL https://deb.nodesource.com/setup_14.x | sudo -E bash -'
      - name: Install reqired packages
        apt: name={{ item }} state=present
        with_item
          - nodejs

ansible-playbook -i /var/inventory /var/play.yml


production-weight-apppostgrsql.postgres.database.azure.com
## admin


sudo su
apt update -y ; apt install ansible -y ; apt upgrade -y

<!-- ssh -i id_rsa.pub adminuser@sysadmin
ssh -i id_rsa.pub adminuser@168.62.169.29 -->
# no root login!

cd ~/.ssh
ssh-keygen -t ed25519 -C "ansible"

# double enter, etc. look into it.

10.0.20.4
10.0.20.5
10.0.20.9

ssh-copy-id -i adminuser@10.0.20.5
ssh-copy-id -i adminuser@10.0.20.4
ssh-copy-id -i adminuser@10.0.20.9

 ssh-copy-id -i ~/.ssh/id_ed25519.pub 

## slaves

ssh 10.0.20.4
ssh 10.0.20.5
ssh 10.0.20.9

P@$$w0rd1234!

sudo su
apt update -y
apt upgrade -y

<!-- python3 is allready installed on ubuntu 20 -->


# press i

# PubkeyAuthentication no -> PubkeyAuthentication yes
sudo su
vim /etc/ssh/sshd_config
service ssh restart
systemctl reload sshd
systemctl status sshd
exit; exit 

MASTER

10.0.20.4
10.0.20.5
10.0.20.9

sudo vim /etc/ansible/hosts

----------- GUIDE
https://www.youtube.com/watch?v=-Q4T9wLsvOQ
ip a under inet - yoour ip

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

sudo nano inventory
[clients]
10.0.20.4
10.0.20.5

ssh-keygen -t ed25519 -C "tower"

ssh-copy-id -i ~/.ssh/tower.pub 10.0.20.4
ansible all --key-file ~/.ssh/id_ed25519.pub -i inventory -m ping
ansible all --key-file ~/.ssh/tower -i inventory -m ping

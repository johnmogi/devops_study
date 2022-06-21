## admin
apt update -y ; apt install ansible -y ; apt upgrade -y
ssh-keygen -y; 
# double enter, etc. look into it.
ssh-copy-id -i azureuser@10.0.20.5

## slaves
azureuser@10.0.20.5
# P@$$w0rd1234!
sudo su 
apt update -y
apt upgrade -y 
apt install software-properties-common
apt install python

vim /etc/ssh/sshd_config

# press i

# PubkeyAuthentication no -> PubkeyAuthentication yes
service ssh restart ; systemctl reload sshd

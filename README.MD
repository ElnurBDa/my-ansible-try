# Install Ansible
python3 -m venv .venv 
.venv/bin/activate
pip3 install ansible

# Preparation of Environment
```bash
cd ubuntu
docker compose build
docker compose up -d

ssh-keygen -t rsa -b 2048
# Specify Path: ssh/idrsa

ssh-copy-id -i ssh/id_rsa ansible@172.19.0.2
ssh-copy-id -i ssh/id_rsa ansible@172.19.0.3
ssh-copy-id -i ssh/id_rsa ansible@172.19.0.4
ssh-copy-id -i ssh/id_rsa ansible@172.19.0.5

# Or transfer id_rsa to ~/.ssh/ and go without -i
```

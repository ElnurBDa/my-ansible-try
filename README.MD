# Why
I learn ansible, that is why.

## Sources:
- Documentation
- Ansible: Up and Running, 3rd Edition

---

# Install Ansible
python3 -m venv .venv 
.venv/bin/activate
pip3 install ansible

# Preparation of Environment (Docker)
```bash
cd ubuntu
docker compose build
docker compose up -d

ssh-keygen -t rsa -b 2048
ssh-copy-id ansible@172.19.0.X
# and do the copy for each one
```

# Preparation of Environment (Vagrant)
```bash
vagrant init ubuntu/focal64
vagrant up
vagrant ssh-config
```


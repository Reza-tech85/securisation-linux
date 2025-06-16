# 🔐 Sécurisation d'une machine Linux (Ubuntu)

## Objectif :
Apprendre à sécuriser une machine Linux étape par étape. J'utilise une machine virtuelle Ubuntu pour m'entraîner.

## Étapes que j’ai suivies :

1. **Mettre à jour le système**
```bash
sudo apt update && sudo apt upgrade -y
adduser reza
usermod -aG sudo reza
passwd -l root
sudo ufw enable
sudo ufw status
sudo ufw allow OpenSSH
sudo systemctl list-unit-files --type=service

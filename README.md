FAZENDO DOWNLOAD DO INSTALADOR & INICIANDO A PRIMEIRA INSTALAÇÃO (USAR SOMENTE PARA PRIMEIRA INSTALAÇÃO):

```bash
sudo apt install -y git && git clone https://github.com/brunin1728/instalodordeploy-main.git && sudo chmod -R 777 instalodordeploy-main && cd instalodordeploy-main && sudo ./install_primaria
```

ACESSANDO DIRETORIO DO INSTALADOR & INICIANDO INSTALAÇÕES ADICIONAIS (USAR ESTE COMANDO PARA SEGUNDA OU MAIS INSTALAÇÃO:
```bash
cd && rm -rf instalodordeploy-main && git clone https://github.com/brunin1728/instalodordeploy-main.git && sudo chmod -R 777 instalodordeploy-main && cd instalodordeploy-main && sudo ./install_instancia
```

sudo su - root <<EOF
  useradd -m -p $(openssl passwd -crypt Bruno280989) -s /bin/bash -G sudo deploy
  usermod -aG sudo deploy
EOF


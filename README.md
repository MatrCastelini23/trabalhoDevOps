# Trabalho DevOps CI/CD

Aluno: Matheus Janoca Castelini
R.A: 250289

## Requisitos para conclusão do trabalho.

### Maquina Virtual de Ubuntu Server.
- Instalação concluída no Oracle VirtualBox.
- Acesso via SSH configurado através:
    - sudo apt isntall openssh-server -y
    - Criado redirecionamento de portas em configurações avançadas de redes do virtualBox

### Git Actions -> Runners
- Adição de new self-hosted runner no GitHub (Linux)
- Passo a passo fornecido pelo GitHub feito dentro do Ubuntu Server (através do acesso SSH). 
- Configurar como um serviço do sistema para rodar em segundo plano.
- sudo ./svc.sh install
    - sudo ./svc.sh start
    - sudo ./svc.sh status para verificar se o serviço está rodando em segundo plano


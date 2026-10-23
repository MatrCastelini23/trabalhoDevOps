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

### Workflow de Deploy

Este WorkFlow sempre é disparado ao clicar no botão dentro da sua action no github.

O Workflow de Deploy possui um trabalho com três passos:
- Checando a verão mais nova do código
> Checa a versão mais nova do código. 
- Descendo a Versão anterior
> Derruba o container antigo
- Subindo Versão mais nova
> Sobe o container novamente com a versão mais nova
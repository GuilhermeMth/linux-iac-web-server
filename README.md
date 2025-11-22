# linux-iac-web-server

Script shell (IaC) simples para automatizar a instalação e configuração de um servidor web básico em Linux.

## O que é
Um script que instala e configura um servidor HTTP, cria uma página index de exemplo e habilita o serviço. Feito para ser um ponto de partida rápido.

## Pré-requisitos
- Linux (Debian/Ubuntu e similares recomendados)
- Acesso root ou sudo

## Uso rápido
1. Clone o repositório:
```bash
git clone https://github.com/GuilhermeMth/linux-iac-web-server.git
cd linux-iac-web-server
```

2. Torne o script executável e rode:
```bash
chmod +x iac.sh
sudo ./iac.sh
```

Ou execute diretamente com bash:
```bash
sudo bash iac.sh
```

## Personalização (opcional)
Edite variáveis no início do script ou exporte variáveis de ambiente antes de executar. Exemplo:
```bash
WEB_DIR=/srv/meusite SERVER_PORT=8080 sudo ./iac.sh
```

## Verificação
- Verifique o serviço:
```bash
sudo systemctl status nginx    # ou apache2/httpd conforme o script escolher
```
- Teste:
```bash
curl http://localhost:80
```

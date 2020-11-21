# docker-alpine-php

Exemplo de container para rodar aplicações Laravel/Lumen

#### Containers
- [x] fmp
- [x] nginx
- [x] mysql

#### Features
- [x] PHP GD lib instalado
- [x] Iniciar MySQL com banco de dados usando um arquivo ```dump.sql```
- [x] Custumização das configurações do ```php.ini```
- [x] Controle de pool ```fmp-pool.conf```
- [x] Custumização das Configurações do Nginx ```nginx.conf```

#### Resolução de Erros

Caso você esteja rodando docker no Windows e estiver enfrentando esse erro:
```ERROR: for db  Cannot start service db: OCI runtime create failed: container_linux.go:349: starting container process caused "process_linux.go:449: container init...```

Considere remover esstas linhas do ```docker-compose.yml```
- "/etc/timezone:/etc/timezone:ro"
- "/etc/localtime:/etc/localtime:ro"

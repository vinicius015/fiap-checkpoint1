# fiap-checkpoint1

Aplicação Java proposta como Checkpoint 1 do primeiro semestre da matéria de Engenharia Web e Microserviços

## Pré-requisitos

- Java 17+
- Docker 
- Acesso a internet
- Acesso ao Docker Hub

# Instalação

#### Clone

```
git clone https://github.com/vinicius015/fiap-checkpoint1.git
```

## Execução


#### Docker

* Criação de imagem

```
docker build -t ping .
```

* Executar container

spring.profiles.active=dev

```
docker run -d -p 8080:8080 -e PROFILE=<prd|dev|stg> fiap-checkpoint1
```

#### Navegação

- Base

http://localhost:8080

- Endpoint que retorna string "Pong em dev" no ambiente dev
- Endpoint que retorna string "Pong em prd" no ambiente prd
- Endpoint que retorna string "Pong em stg" no ambiente stg

http://localhost:8080/ping 

## Features (Funcionalidades)

- Múltiplos profiles

## Contatos

- Gabriel Penna de Lima - rm94841@fiap.com.br
- Vinicius dos Santos Amaral - rm96108@fiap.com.br

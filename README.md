# Conversão de Temperatura

## Sobre o Projeto
Este projeto é um exemplo de aplicação Node.js para conversão de temperatura, com foco em demonstrar a criação de ambientes com containers.

- **Linguagem:** Node.js
- **Porta exposta:** 8080

## Passo a Passo

### 1. Construir a imagem Docker

```sh
docker build -t oalexandrino/conversao-temperatura-kind:v1 .
```

### 2. Criar o cluster KIND e adicionar a imagem local

```sh
kind load --name meu-cluster docker-image oalexandrino/conversao-temperatura-kind:v1
```

### 3. Aplicar o deploy no Kubernetes

```sh
kubectl apply -f .\deploy.yaml
```


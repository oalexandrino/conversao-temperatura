# Projeto conversão de temperatura

### Sobre o projeto
O projeto conversão de temperatura é um projeto desenvolvido em NodeJS. O projeto tem como objetivo ser um exemplo para a criação de ambiente com containers usando NodeJS.

### Observações do projeto
A aplicação é exposta usando a porta 8080

## Passo a passo

# Criar cluster
## adicionar imagem local no cluster:

 kind load --name meu-cluster docker-image oalexandrino/conversao-temperatura-kind:v1

## Aplicar o deploy

kubectl apply -f .\deploy.yaml

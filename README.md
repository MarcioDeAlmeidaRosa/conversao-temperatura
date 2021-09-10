# Conversão de Temperatura
Api responsável por efetuar a conversão Celsius para Fahrenheit e Fahrenheit para Celsius.

## Build da imagem

Executar via prompt de comando dentro da pasta /src: 
`docker build --build-arg ARG_NODE_PORT=8080 -t marcioalmeidarosa/conversao-temperatura:1.0 .`. 
Este comando irá gerar uma imagem local que conserá ter acesso executando o comando: 
`docker images marcioalmeidarosa/conversao-temperatura`.

## Executando o container com a imagem local

Executar via prompt de comando para executar o container com a imagem gerada: 
`docker run --name=api_conversao-temperatura_node --env-file ./.env -p 8080:8070 -d marcioalmeidarosa/conversao-temperatura:1.0`. 
Este comando irá startar um container que poderá ser visualizado com o comando: 
`docker images marcioalmeidarosa/conversao-temperatura`.

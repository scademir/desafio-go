Este é o código desenvolvido para o primeiro desafio do módulo Docker do curso Full Cycle. O objetivo é criar uma imagem que rode um executável que exiba a mensagem Full Stack Rocks!! desenvolvido em GoLang. A imagem deve ter no máximo 2Mb e deve estar disponível no dockerhub.

Usando o código-fonte

Após clonar o projeto, navegue pelo terminal até a pasta com os arquivos e faça o build da imagem

docker build -t my-golang-app-alpine .

Em seguida, rode o container com a imagem que acabou de criar

docker run --rm --name my-running-app my-golang-app-alpine

Você deve receber a mensagem Full Cycle Rocks!! em seu terminal

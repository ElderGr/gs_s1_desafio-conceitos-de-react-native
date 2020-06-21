# Desafio GoStack: Conceitos básicos de React Native
Projeto desenvolvido durante a Semana 1 do bootcamp GoStack, onde conceitos básicos como estado, imutabilidade e componentização no React Native foram exercitados.

## ⚙ Pré-requisitos
Para a execução do projeto em seu ambiente local é necessário possuir instalado: 

- NodeJS em sua versão LTS
> https://nodejs.org/en/

- Configurar o ambiente local mobile, seguindo os passos abaixo 
> https://react-native.rocketseat.dev/

## 🛠 Guia de instalação do projeto
1. Faça download do projeto do github
2. Após ter feito download do projeto, acesse o diretorio raiz do mesmo via linha de comando
3. No terminal, execute o comando npm install para instalar as dependências do projeto (Caso você tenha o yarn instalado em sua máquina, execute apenas yarn para a instalação das dependencias)
4. Com o ambiente mobile configurado e com um emulador android/ios em execução, ou um device conectado via usb, execute o comando _react-native run-android_ ou _react-native run-ios_ para IOS. Caso você possua mais de um device conectado ou emulador em execução passe o nome do dispositivo no final dos comandos citados acima.

## 📃 Guia de utilização
Link para a API que o APP está consumindo
> https://github.com/ElderGr/gs_s1_desafio-conceitos-de-node

No caminho src/services/api.js teremos o arquivo de configuração para as requisições a API. Será necessário realizar alterações no valor de _baseURL_ baseado na forma que o ambiente mobile está sendo utilizado

**Device USB IOS/Android**: 
Caso você esteja com um device conectado via USB tanto Android quanto IOS, a string deverá seguir o padrão http://_ip_:_port_, onde ip é o ip do pc que está sendo executada a api e port a porta que está sendo utilizada. É necessário que o device esteja na mesma rede da pc.

**Device Android**:
Execute o comando adb reverse tcp:3333 tcp:3333 e defina o valor da _baseURL_ como http://localhost:3333

**Device IOS**:
Defina o valor da _baseURL_ como http://localhost:3333

## 📋 Comandos disponíveis
* start: execução do app em seu device ou emulador após o bundle ter sido gerado
* test: execução dos testes validando o desenvolvimento do APP

## 📙 Enunciado
Todo o desafio foi realizado baseado no enunciado: 
> https://github.com/Rocketseat/bootcamp-gostack-desafios/tree/master/desafio-conceitos-reactjs
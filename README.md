# Api usando o Faker

Este projeto é um aplicativo React Native que exibe uma lista de usuários gerados aleatoriamente. Os dados são armazenados em um servidor JSON local e podem ser editados diretamente no app.

## Requisitos

Antes de rodar o projeto, certifique-se de ter instalado:

- [Node.js](https://nodejs.org/)
- [Expo CLI](https://docs.expo.dev/get-started/installation/)
- [JSON Server](https://github.com/typicode/json-server)

## Instalação

1. Clone este repositório:
   ```sh
   git clone https://github.com/Yago-Aura/Api_Fetch.git
   cd Api_Fetch
   ```

2. Instale as dependências do projeto:
   ```sh
   npm install
   ```
   em ambas as pastas

## Gerando Dados com Faker.js

1. Instale o Faker.js e o Lodash:
   ```sh
   npm install @faker-js/faker lodash
   ```

2. Execute o script para gerar dados simulados:
   ```sh
   node generateData.js
   ```
   na pasta backend
   O script utiliza **Faker.js** para criar usuários fictícios com nomes, avatares, endereços e e-mails.

## Rodando o Servidor JSON

1. Inicie o JSON Server:
   ```sh
   npx json-server --watch db.json --port 3000
   ```

Se estiver rodando em um dispositivo físico, substitua `localhost` pelo IP da sua máquina no código.

## Rodando o App

1. Inicie o Expo:
   ```sh
   npx expo start
   npx expo start --tunnel
   ```
   o tunnel é acaso se usar redes diferentes

2. Escolha uma das opção:
Emular na web aperte a tecla "w"

## Estrutura do Projeto

```
Api_Fetch/
├── App.js              # Componente principal do React Native
├── UserList.js         # Tela que exibe a lista de usuários
├── UserDetail.js       # Tela de detalhes e edição de um usuário
├── generateData.js     # Script para gerar dados simulados
├── db.json             # Banco de dados local gerado pelo JSON Server
├── package.json        # Dependências do projeto
```

## Funcionalidades
- Exibição de uma lista de usuários com imagens e detalhes
- Atualização dos dados dos usuários diretamente no app
- Interface responsiva com suporte a temas escuros

## Tecnologias Utilizadas
- **React Native** (Expo)
- **React Navigation** para navegação
- **Axios** para consumir a API
- **JSON Server** para simular um backend
- **Faker.js** para gerar dados aleatórios
- **Lodash** para manipulação de listas

## Como usar  corretamente
-Usar as duas pastas simultaneamente em duas paginas do vs code

## Autor
Criado por [Yago-Aura]


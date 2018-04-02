# workshop-web-ipea-2018-04
Workshop de Desenvolvimento Web, IPEA, Abril/2018

## Introdução / Definições:

- O que o browser "lê"?
- MPA/MVC vs SPA
    - [SPAs vs MPAs/MVC - Are Single Page Apps always better? - Academind](https://www.youtube.com/watch?v=F_BYg2QGsC0)

- Definições:
    - SPA (Web App)
    - Modular (frontend/backend)

- Problema 1) Como desenvolver rápido, de forma simples, modular e flexível?
    - JavaScripts frameworks (React, Vue, Angular, Aurelia... Riot.js)
    - Mas pq?
        - [JavaScript in 2017: You might (not) need a framework - David Vujic - NDC Conferences](https://www.youtube.com/watch?v=dGws1pMWzCI)
    - O que é preciso para estruturar um Web App?
        - [The Frontend Is A Full Stack - Coding Tech](https://www.youtube.com/watch?v=0c9OC9NBsro)

- Problema 2) Como otimizar a carga do Web App?
    - Webpack

- Problema 3) Como gerenciar o estado (state) da aplicação?
    - Redux

- Problema 4) Como programar de forma organizada, estruturada, simples e permitir chamadas assíncronas?
    - Redux-saga

- Problema 5) Como escrever um código com os rescursos mais modernos à nossa disposição?
    - Babel/Webpack
    - Typescript*

- Resumo:
    - Tudo tem um porquê
        - SPA
        - Riot.js (Curso Udemy)
        - Webpack
            - https://webpack.js.org/
            - [Webpack 2 Basics - Academind](https://www.youtube.com/watch?v=GU-2T7k9NfI&list=PL55RiY5tL51rcCnrOrZixuOsZhAHHy6os)
            - [Webpack 2 - Ihatetomatoes](https://www.youtube.com/watch?v=JdGnYNtuEtE&list=PLkEZWD8wbltnRp6nRR8kv97RbpcUdNawY)
        - Redux/redux-saga
            - Wes Bos Curso Redux
            - https://redux.js.org/
            - https://redux-saga.js.org/
        - Babel
    - Entender tudo, linha a linha, saber o porquê


## Por que o Riot.js?

- Todos os principais recursos dos demais frameworks*
    - **Componentes**!!!!!!!
    - "Virtual DOM"
    - Geração de HTML em função do state
    - Lifecycle
- Diferenciais
    - Leve (MUITO)
    - Sintaxe IGUAL a HTML normal
    - Código FACIL de escrever e de ler
    - Compatibilidade nativa com componentes externos (jQuery, etc...)

## Rápida Rrevisão

### - Riot.js

- Client side compilation:
    - riot+compiler.min.js
        - transforma o `.tag` em uma função javascript `riot.tag2(...)`
    - riot.min.js
        - executa a função `riot.tag2(...)`
        - o retorno dessa função -> carrega no DOM

- Pre-compiled: Como nós iremos usar?
    - Node.js irá compilar e gerar o arquivo `.js` com as funções `riot.tag2(...)`
    - Webpack irá juntar esse `.js` com essas funções `riot.tag2(...)`, no `bundle.js`

### - Transpile Code (Transpilar o código)

- Babel
- Typescript
- SASS / LESS

### - Comandos de Terminal

- Flags vs `.config`

### - Webpack

- O que faz?
- Busca "em árvore" a partir de ponto de entrada `entry`
- Saída de pacotes únicos para cada tipo de arquivo (`.js`, `.css`, imagens, etc...)


## Configurar o ambiente

- nvm

- vscode

- `package.json`

```
npm init -y
```

- Configurar o Webpack

- `npx`
    - `riot --config riot.config`
    - `webpack`

- Montar os scripts no npm `package.json` com a flag watch `-w`




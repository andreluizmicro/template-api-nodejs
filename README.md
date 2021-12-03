### Configuração Geral do Projeto

### PASSOS

- 1 - npm init ou  yarn init -y
- 2 - yarn add typescript -D
- 3 - yarn add @types/typescript -D
- 4 - yarn add express
- 5 - yarn add @types/express -D
- 6 - tsc --init 

### Configuração do ESLINT e PRETTIER

[https://www.notion.so/ESLint-e-Prettier-Trilha-Node-js-d3f3ef576e7f45dfbbde5c25fa662779#eaf6e8bdcabc4d809cdae302e29750da](https://www.notion.so/ESLint-e-Prettier-Trilha-Node-js-d3f3ef576e7f45dfbbde5c25fa662779#eaf6e8bdcabc4d809cdae302e29750da)

1 - Instalar a extensão do ESLint no vscode
2 - Uma outra configuração que é geral e precisamos fazer para o **VSCode** formatar o código sempre que salvarmos algum arquivo é adicionar uma opção chamada `codeActionsOnSave` nas configurações, assim como mostrado abaixo:

Usando Ctrl + , -> acessar as configurações do VSCODE e adicionar: 

    "editor.codeActionsOnSave": {
      "source.fixAll.eslint": true
    }

- yarn add eslint -D - yarn add eslint -D --ignore-engines
- yarn eslint --init

### Para configuração escolhemos as opções abaixo

- To check syntax, find problems and enforce code style
- javascript modules (import/export)
- none of these
- use typescript
- node
- use a popular style guide
- Airbnb
- JSON

Precisamos também instalar um plugin que irá nos auxiliar a organizar a ordem dos imports dentro dos arquivos e outro para permitir importações de arquivos TypeScript sem que precisemos passar a extensão do arquivo:

- yarn add -D eslint-plugin-import-helpers eslint-import-resolver-typescript --ignore-engines

Com as dependências instaladas vamos criar na raiz do projeto um arquivo .eslintignore com o conteúdo abaixo para ignorar o Linting em alguns arquivos:

    /*.js
    node_modules
    dist

yarn add prettier eslint-config-prettier eslint-plugin-prettier -D
Sequência de passos para setup de projetos Node com TypeScript para Windows.

Esse template pode ser clonado e executado (comando: "npm install") para instalação das dependências. Isso garante que os arquivos de configuração "tsconfig.json" e "eslintrc.json" sejam iguais.

Pré-requisitos do ambiente de desenvolvimento:

- Visual Studio Code (ou outro editor de texto)
- Node.js + NPM
- Git
- Compilador TypeScript instalado globalmente - `npm i -g typescript`
- Simulador de runtime TypeScript instalado globalmente - `npm i -g ts-node`
- Biblioteca de tipos do Node.js instalada globalmente - `npm i -g @types/node`
## Passo a passo para um novo projeto
Após criar a pasta para seu projeto:
1. `git init` - Inicia repositório git na pasta
2. Vincular o repositório Git a um repositório remoto (geralmente hospedado no GitHub)
3. Criar arquivo `.gitgnore` e registrar nele a pasta `node_modules/`
4. `npm init -y` - Cria o arquivo `package.json`, iniciando projeto Node.js
5. Instalar dependências de desenvolvimento
   1. `npm i -D typescript` - Dependência local do TypeScript para desenvolvimento
   2. `npm i -D ts-node` - Simulador do runtime TypeScript
   3. `npm i -D eslint` - Linter para o TypeScript
   4. `npm i -D @types/node` - Biblioteca de tipos para os módulos nativos do Node.js
6. `tsc --init` - Cria o arquivo `tsconfig.json`, com as configurações do TypeScript para o projeto
7. `npm init @eslint/config` - Cria o arquivo de configuração do ESLint
8. `npm i -D dotenv` - Instala a dependência do pacote `dotenv` para interpretação de variáveis de ambiente em ambiente de desenvolvimento
9. Criar o arquivo `.env` e preencher com `NODE_ENV=development`
10. Alterar os arquivos `tsconfig.json` e `.eslintrc.json` conforme desejado
11. Alterar o arquivo `package.json` conforme necessidade:
    1. Alterar o caminho do arquivo principal (*main*) para o arquivo de saída principal emitido pelo TypeScript. Por ex.: `./dist/index.js`
    2. Inserir scripts dos comandos `start`, `dev` e `build` desejados
    
    Repositório de exercícios do curso de Web Moderno Completo com JavaScript da Udemy.

IDE utilizada: Visual Studio Code.

Sequência de etapas para setup de projetos Node com TypeScript para Windows.

Esse template pode ser clonado e executado (comando: "npm install") para instalação das dependências. Isso garante que os arquivos de configuração "tsconfig.json" e "eslintrc.json" sejam iguais.

Pré-requisitos do ambiente de desenvolvimento:

- Visual Studio Code (ou outro editor de texto);
- Node.js + npm;
- Git;
- Compilador TypeScript instalado globalmente ("npm install -g typescript");
- Simulador de runtime TypeScript instalado globalmente ("npm install -g ts-node");
- Biblioteca de tipos do Node.js instalada globalmente ("npm install -g @types/node");

Etapas para criação de um novo projeto

- Criar uma pasta para o projeto;
- Iniciar o repositório "git" na pasta ("git init");
- Vincular o repositório "git" a um repositório remoto (sugestão: GitHub);
- Criar o arquivo "gitignore" e incluir a pasta "node_modules/";
- Criar o arquivo "package.json" ("npm init -y") para iniciar o projeto Node.js;
- Criar o arquivo ".env" e preencher com "NODE_ENV=development".

Instalação das dependências de desenvolvimento:

- "npm i -D typescript" (dependência local do TypeScript para desenvolvimento);
- "npm i -D ts-node" (simulador do runtime TypeScript);
- "npm i -D eslint" (linter para o TypeScript);
- "npm i -D @types/node" (biblioteca de tipos para os módulos nativos do Node.js);
- "tsc --init" (cria o arquivo "tsconfig.json", com as configurações do TypeScript para o projeto);
- "npm init @eslint/config" (cria o arquivo de configuração do ESLint);
- "npm i -D dotenv" (instala a dependência do pacote "dotenv" para interpretação de variáveis de ambiente no ambiente de desenvolvimento);

Observações:

- Alterar os arquivos "tsconfig.json" e "eslintrc.json" conforme necessidade;

- Alterar o arquivo "package.json" conforme necessidade. Exemplos:
   * Alterar o caminho do arquivo principal (main) para o arquivo de saída principal emitido pelo TypeScript;
-Por ex.: `./dist/index.js`
    2. Inserir scripts dos comandos `start`, `dev` e `build` desejado
 
IDE utilizada: Visual Studio Code.

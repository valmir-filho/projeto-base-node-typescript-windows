# Sequência de etapas para setup de projetos Node com TypeScript para Windows.

* Esse template pode ser clonado e executado (comando: "npm install") para instalação das dependências. Isso garante que os arquivos de configuração "tsconfig.json" e "eslintrc.json" sejam iguais.

## Pré-requisitos do ambiente de desenvolvimento:

- Visual Studio Code (ou outro editor de texto);
- Node.js + npm;
- Git;
- Compilador TypeScript instalado globalmente ("npm install -g typescript");
- Simulador de runtime TypeScript instalado globalmente ("npm install -g ts-node");
- Biblioteca de tipos do Node.js instalada globalmente ("npm install -g @types/node").

## Etapas para criação de um novo projeto:

- Criar uma pasta para o projeto;
- Iniciar o repositório "git" na pasta ("git init");
- Vincular o repositório "git" a um repositório remoto (sugestão: GitHub);
- Criar o arquivo ".gitignore" e incluir as pastas: "node_modules/" e ".vscode/";
- Criar o arquivo "package.json" ("npm init -y") para iniciar o projeto Node.js;
- Criar o arquivo ".env" e preencher com "NODE_ENV=development".

## Instalação das dependências de desenvolvimento:

- "npm i -D typescript" (dependência local do TypeScript para desenvolvimento);
- "npm i -D ts-node" (simulador do runtime TypeScript);
- "npm i -D eslint" (linter para o TypeScript);
- "npm i -D @types/node" (biblioteca de tipos para os módulos nativos do Node.js);
- "tsc --init" (cria o arquivo "tsconfig.json", com as configurações do TypeScript para o projeto);
- "npm init @eslint/config" (cria o arquivo de configuração do ESLint). Após a instalação, definir as seguintes configurações:
  - How would you like to use EsLint? "To check syntax, find problems, and enforce code style";
  - What type of modules does your project use? "JavaScript modules (import/export)";
  - Which framework does your project use? "None of these";
  - Does your project use TypeScript? "Yes";
  - Where does your code run? "✓Browser ✓Node";
  - How would you like to define a style for your project? "Answer questions about your style";
  - What format do you want your config file to be in? "JSON";
  - What style of identation do you use? "Tabs";
  - What quotes do you use for strings? "Double";
  - What line endings do you use? "Windows";
  - Do you require semicolons? "Yes";
  - Would you like to install them now? "Yes";
  - Which package manager do you want to use? "npm";
- "npm i -D dotenv" (instala a dependência do pacote "dotenv" para interpretação de variáveis de ambiente no ambiente de desenvolvimento).

## Observações:

- Alterar os arquivos "tsconfig.json" e "eslintrc.json" conforme necessidade;

- Alterar o arquivo "package.json" conforme necessidade. Exemplos:
  - modificar o caminho do arquivo principal (main) para o arquivo de saída principal emitido pelo TypeScript (exemplo: "./build/index.js");
  - inserir scripts dos comandos "start", "dev" e "build".
 
### IDE utilizada: Visual Studio Code.

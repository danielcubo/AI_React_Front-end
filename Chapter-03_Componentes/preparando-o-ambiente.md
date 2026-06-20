## [![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)](https://nodejs.org/pt-br/download)


### `nvm` Node Version Manager
Gerenciador de versões do Node.js

Ele atua diretamente no programa principal.

Por usar o nvm?
- **Isolamento de projetos**: você pode rodar um projeto usando versões diferentes para diferentes projetos.
- **Alternância rápida**: Com um único comando, como `nvm use 20`, você vuda a versão ativa do Node no seu terminal.
- **Instalação descomplicada**: Não é necessário baixar instaladores manualmente e sobrescrever arquivos. O NVM cuida do download e da configuração correta das variáveis de ambiente.
- **Comandos mais comuns**:
```bash
# Instala uma versão específica do Node.js
nvm install 24

# Seleciona uma versão específica do Node para ser usada.
nvm use 20
```

### [![NPM](https://img.shields.io/badge/NPM-%23CB3837.svg?style=for-the-badge&logo=npm&logoColor=white)](https://www.npmjs.com/) Node Package Manager
Gerenciador de pacotes do Node.js


Ele atua nos acessórios que você coloca dentro do projeto, que são as bibliotecas e códigos de terceiros.

O NPM descobre o que precisa baixar para o seu projeto olhando para um arquivo especial chamado `package.json`.

Esse arquivo funciona como a "lista de compras" do seu projeto. Ele fica na pasta principal e diz ao NPM exatamente quais códigos de terceiros (chamados de dependências) o seu site precisa para funcionar.

Quando você inicia um projeto, o `package.json` guarda as informações básicas dele.

- **Comandos mais comuns**:
```bash
# Iniciar um projeto usando Node.js
npm init

# Instalar a biblioteca React
npm install react

# Remover a biblioteca React
npm uninstall react

# Instalar um projeto que você baixo da internet
npm install

# iniciar o projeto
npm run start

# iniciar o projeto
npm start

# iniciar o projeto
npm run dev

# iniciar o projeto
npm run preview
```

1. `npm start` (Modo produção/inicialização)
- **Para quem server**: Para o servidor de internet que vai mostrar o site para o público.
- **O que faz**: Liga o siste em modo de alta performance. Ele não fica vigiando alterações no código, porque o site já está pronto e não deve ser mexido. Ele apenas entrega as páginas prontas o mais rápido possível para os usuários.
- **Ferramentea**: era muito usado no antigo *Create React App*. No Vite, o comando equivalente para testar o site finalizado localmente costuma ser o `npm run preview`
2. `npm run dev` (Modo desenvolvimento)
- **Para que serve**: Para você, o programador, usar no dia a dia.
- **O que faz**: Liga um servidor que fica vigiando o seu código. Se você alterar uma cor ou um texto no arquivo e salvar, o site atualiza na tela do navegador instantaneamente.
- **Ferramenta**: É o comando padrão usado pelo **Vite** pra você construir o site.


### `npx` Node Package Executer
É uma ferramenta que serve para executar comandos de bibliotecas do Node.js sem que você precise instalar essas ferramentas de forma permanente no seu computador.

Ele vem instalado automaticamente junto com o NPM. A principal diferença é que NPM baixa coisas, e o NPX roda coisas.

O NPX é usado para criar projetos com React.

A comunidade React não recomenda usar o comando `npx create react app`.

O jeito mais moderno é usar uma ferramenta chamada **[⚡ Vite](https://vite.dev/)**.

Ela usa novas tecnologias do Node.js e dos navegadores para carregar apenas a parte do código que você está usando no momento.

Para criar seu projeto React, digite:
```bash
npx create-vite@latest meu-app-react --template react
```

**O que acontece depois de rodar esse comando?**
1. O NPX vai buscar o criador de projetos do Vite na internet.
2. Ela vai criar uma pasta chamada `meu-app-react` com toda a estrutura do React pronta.
3. O NPX some do computador e não deixa lixo instalado.

**E quando eu uso o NPM?**

Assim que o NPX terminar de criar as pastas, você vai entrar na pasta do projeto e usar o NPM para trabalhar neles. Os comandos que você vai digitar em seguida são:
```bash
# 1. Entra na pasta que o npx criou
cd meu-app-react

# 2. Usa o NPM para instalar os códigos internos do React
npm install

# 3. Usa o NPM para ligar o servidor e ver o site no navegador
npm run dev
```

## Ferramentas online para criar Projetos React
- [https://stackblitz.com/](https://stackblitz.com/)
- [https://codesandbox.io/](https://codesandbox.io/)
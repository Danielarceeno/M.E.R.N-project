Pequeno projeto para desenvolvimento M.E.R.N

# 💻 Tech Stack:
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white) ![Express.js](https://img.shields.io/badge/express.js-%23404d59.svg?style=for-the-badge&logo=express&logoColor=%2361DAFB) ![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB) ![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white) 


# Manual de Utilização do Projeto

## Instruções Passo a Passo 

### Passo 1: Clonando o Repositório /end

Certifique-se de clonar o repositório para sua máquina local. Abra o terminal e navegue até o diretório onde deseja clonar o repositório. Em seguida, execute o seguinte comando:

```bash
git clone <URL_DO_REPOSITORIO>
```
Crie uma pasta:

```bash
mkdir server
```

Depois de clonar, entre no diretório do servidor:

```bash
cd server
```

### Passo 2: Instalando Dependências

Antes de iniciar o servidor, é necessário instalar as dependências do projeto. Execute o seguinte comando no terminal:

```bash
npm install -g nodemon
```

Este comando instalará globalmente o Nodemon, uma ferramenta útil para o desenvolvimento de aplicações Node.js. Em seguida, instale as dependências do projeto:

```bash
npm install express body-parser bcrypt cors dotenv gridfs-stream multer multer-gridfs-storage helmet morgan jsonwebtoken mongoose
```

Se ocorrer algum erro durante a instalação, tente excluir os arquivos `package-lock.json` e `package.json` e execute novamente o comando de instalação.

### Passo 3: Configurando o Arquivo `package.json`

Após instalar as dependências, é necessário configurar o arquivo `package.json`. Execute o seguinte comando para inicializar um arquivo `package.json`:

```bash
npm init -y
```

Em seguida, abra o arquivo `package.json` e adicione o seguinte código abaixo da chave `"main"`:

```json
"type": "module",
```

Isso é necessário devido a um problema com os módulos ES6. Ainda no arquivo `package.json`, adicione o seguinte dentro da chave `"scripts"`:

```json
"start": "nodemon index.js"
```

### Passo 4: Criando o Arquivo `.env`

Por fim, crie um arquivo `.env` seguindo o exemplo do arquivo `.env.example` fornecido. Este arquivo será usado para configurar variáveis de ambiente necessárias para o funcionamento do servidor.

-------------------------------------------------------------------
## Instalação do Cliente (Client)

Para começar, na pasta principal do seu projeto, execute os seguintes comandos:

1. Crie o aplicativo React utilizando:

    ```bash
    npx create-react-app client
    ```

2. Em seguida, entre no diretório recém-criado:

    ```bash
    cd client
    ```

3. Instale as dependências necessárias para o cliente:

    ```bash
    npm i react-redux @reduxjs/toolkit redux-persist react-dropzone dotenv formik yup react-router-dom@6 @mui/material @emotion/react @emotion/styled @mui/icons-material
    ```

Feito isso, sempre que desejar iniciar o servidor, certifique-se de iniciar tanto o servidor quanto o cliente. Você pode fazer isso executando `npm start` nos respectivos diretórios.

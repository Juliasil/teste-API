# teste-API
Desafio técnico para empresa TipsCode BackEnd e FrontEnd: API com dois Endpoints para autenticação de usuário (username e password) e dois clientes - um HTML/CSS/JS e outro em ReactJS. Dados são armazenados em MongoDb e disponibilizados em formato JSON.
# Projeto de API de Autenticação

Este é um projeto de API de autenticação simples que permite o registro de usuários e a autenticação de usuários com base em seus e-mails e senhas. Os dados dos usuários são armazenados em um banco de dados MongoDB.

## Endpoints

A API possui os seguintes endpoints:

### 1. Registro de Usuário

- **Endpoint**: `/register`
- **Método**: POST
- **Descrição**: Permite que um usuário se registre fornecendo um nome, um e-mail e uma senha.
- **Entrada**: JSON com os campos `name`, `email` e `password`.
- **Validações**: Os campos `name`, `email` e `password` são obrigatórios. O campo `email` deve ser único.
- **Saída de Sucesso**: JSON com uma mensagem de confirmação.
  ### 2. Autenticação de Usuário

- **Endpoint**: `/login`
- **Método**: POST
- **Descrição**: Permite que um usuário faça login fornecendo seu e-mail e senha.
- **Entrada**: JSON com os campos `email` e `password`.
- **Validações**: Os campos `email` e `password` são obrigatórios.
- **Saída de Sucesso**: JSON com uma mensagem de sucesso.
- **Saída de Erro**: JSON com mensagens de erro, como senhas incorretas ou e-mails não encontrados.

## Pré-requisitos

Para executar este projeto, você precisará das seguintes dependências:

- Node.js
- MongoDB (com uma instância em execução)
- Dependências do projeto (instaladas via `npm install`)

## Instalação

1. Clone este repositório.
2. Instale as dependências com o comando:

npm install


3. Certifique-se de ter uma instância do MongoDB em execução e configure a URL de conexão no arquivo `index.js` se necessário.

4. Inicie o servidor com o comando:

node index.js


A API estará em execução na porta 3001 por padrão.

## Uso

- Para registrar um novo usuário, faça uma solicitação POST para `/register` com um JSON contendo os campos `name`, `email` e `password`.

- Para fazer login, faça uma solicitação POST para `/login` com um JSON contendo os campos `email` e `password`.









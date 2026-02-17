# Meu Primeiro Backend com Node.js 🚀

Este é um projeto pessoal construído com o objetivo de dar os primeiros passos no desenvolvimento backend. Nele, aprendi a estruturar uma API, entender como funcionam as requisições web e integrar a aplicação a um banco de dados NoSQL utilizando um ORM moderno.

## 🛠️ Tecnologias Utilizadas

* **Node.js**: Ambiente de execução do JavaScript no servidor.
* **Express**: Framework para criar as rotas e gerenciar as requisições HTTP (GET, POST, etc).
* **Prisma ORM**: Ferramenta que facilitou a comunicação com o banco de dados e a criação dos modelos (versão 6.19).
* **MongoDB**: Banco de dados NoSQL em nuvem (Atlas).

## 🧠 O que eu aprendi

- Iniciar um servidor usando Node e Express.
- Criar rotas para receber requisições e devolver respostas estruturadas em JSON.
- Configurar variáveis de ambiente (`.env`) para proteger dados sensíveis.
- Modelar dados utilizando o arquivo `schema.prisma`.
- Conectar e manipular dados no MongoDB através do Prisma Client.

## 💻 Como rodar este projeto na sua máquina

### Pré-requisitos
Antes de começar, você vai precisar ter instalado na sua máquina o Node.js e ter uma conta no MongoDB Atlas para criar o seu próprio banco de dados.

### Passo a Passo

1. **Clone o repositório:**

2. **Acesse a pasta do projeto:**

3. **Instale as dependências:**
    npm install

4. **Configure as variáveis de ambiente:**
    - Crie um arquivo chamado `.env` na raiz do projeto (você pode usar o arquivo `.env.example` como base).
    - Adicione a URL de conexão do seu MongoDB:
    DATABASE_URL="mongodb+srv://SEU_USUARIO:SUA_SENHA@cluster.../NOME_DO_BANCO"

5. **Gere o cliente do Prisma e sincronize o banco:**
    npx prisma generate
    npx prisma db push

6. **Inicie o servidor:**
    node --watch server.js

A API estará rodando! (Geralmente em `http://localhost:3000`, dependendo da sua porta).

## 🔀 Rotas da API

Aqui estão os principais endpoints da aplicação:

| Método | Rota | Descrição |
|---|---|---|
| `GET` | `/users` | Retorna todos os usuários cadastrados. |
| `POST` | `/users` | Cria um novo usuário. |
| `PUT` | `/users/:id` | Atualiza os dados de um usuário específico. |
| `DELETE` | `/users/:id` | Deleta um usuário específico. |

*(Nota: Você pode testar essas rotas usando ferramentas como Insomnia, Postman ou Thunder Client).*
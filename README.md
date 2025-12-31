# 📝 Task Manager — Full Stack Ecosystem

<p align="center">
  <img src="https://img.shields.io/badge/Status-Concluído-success?style=for-the-badge" alt="Status">
  <img src="https://img.shields.io/badge/Deploy-Vercel-black?style=for-the-badge&logo=vercel" alt="Deploy">
  <img src="https://img.shields.io/badge/Database-Supabase-3ECF8E?style=for-the-badge&logo=supabase" alt="Database">
  <img src="https://img.shields.io/badge/API-REST-blue?style=for-the-badge" alt="API REST">
  <img src="https://img.shields.io/badge/Auth-JWT-orange?style=for-the-badge" alt="JWT">
</p>

O **Task Manager** é uma aplicação **Full Stack** focada em produtividade, projetada para gerenciar o ciclo de vida completo de tarefas com **autenticação segura**, **operações CRUD avançadas** e **integração com serviços em nuvem**.

O projeto foi desenvolvido com foco em **boas práticas de arquitetura**, **escalabilidade**, **segurança** e **automação**, sendo ideal para demonstrar domínio prático de um ecossistema moderno de desenvolvimento web.

---

## 📸 Preview do Projeto

<p align="center">
  <img src="https://github.com/IagoRdgs/task-manager/blob/master/frontend/public/image.png" width="100%" alt="Dashboard Preview">
</p>

---

## 🚀 Funcionalidades

### 🔐 Autenticação & Segurança
- Cadastro de usuários
- Login com JWT
- Proteção de rotas via middleware
- Hash de senha
- Controle de sessão

### ✅ Gerenciamento de Tarefas
- Criar, editar e excluir tarefas
- Listagem por usuário autenticado
- Marcação de status (pendente / concluída)
- Validações no backend

### 📊 Experiência do Usuário
- Interface responsiva
- Dashboard intuitivo
- Componentes reutilizáveis

---

## 🛠️ Stack Tecnológica & Arquitetura

### 🖥️ Frontend
- React.js
- Bootstrap
- Axios

### ⚙️ Backend
- Node.js
- Express
- Prisma ORM

### 🗄️ Banco de Dados
- Supabase (PostgreSQL)

### 🔒 Segurança
- JWT (JSON Web Token)

### 🔄 DevOps & Automação
- GitHub Actions
- CI/CD automatizado
- Rotina automatizada para manter o banco ativo

---

## 📂 Estrutura do Projeto

    task-manager/
    ├── frontend/
    │   ├── public/
    │   └── src/
    │       ├── components/
    │       ├── pages/
    │       ├── api/
    │       └── styles/
    │
    ├── api/
    │   ├── prisma/
    │   └── src/
    │       ├── controllers/
    │       ├── middleware/
    │       ├── routes/
    │       └── services/
    │
    ├── .github/
    │   └── workflows/
    │       └── keep-alive.yml
    │
    └── README.md

---

## 🔌 Endpoints Principais da API

### 🔐 Autenticação

    POST /auth/register
    POST /auth/login

### ✅ Tarefas

    GET    /tasks
    POST   /tasks
    PUT    /tasks/:id
    DELETE /tasks/:id

> 🔒 Todos os endpoints de tarefas exigem autenticação JWT.

---

## ⚙️ Pré-requisitos

- Node.js 16+
- npm ou yarn
- Conta no Supabase

---

## 🔑 Variáveis de Ambiente

    SUPABASE_URL=https://seu-projeto.supabase.co
    SUPABASE_ANON_KEY=anon-key-do-supabase
    DATABASE_URL="postgresql://USER:PASSWORD@HOST:PORT/DATABASE?schema=public"
    JWT_SECRET=sua_chave_secreta
    PORT=3333

---

## ▶️ Como Executar Localmente

### Backend

    cd api
    npm install
    npx prisma migrate dev
    npm run dev

### Frontend

    cd frontend
    npm install
    npm start

Frontend: http://localhost:3000  
API: http://localhost:3333  

---

## 🤖 GitHub Actions — Keep Alive (Supabase)

Para evitar que o banco de dados do Supabase entre em modo de inatividade (idle), foi configurado um **workflow automatizado** utilizando **GitHub Actions**.

Esse workflow executa periodicamente uma requisição simples à API ou ao banco de dados, garantindo que o serviço permaneça ativo mesmo em planos gratuitos.

### Características
- Execução agendada (cron)
- Baixo consumo de recursos
- Evita cold start / expiração do banco
- Totalmente automatizado

> Arquivo localizado em `.github/workflows/keep-alive.yml`

---

## 🚢 Deploy

- Frontend: Vercel
- Backend: Render / Railway
- Database: Supabase
- Automação: GitHub Actions

---

## 🧪 Boas Práticas

- Arquitetura desacoplada
- Separação de responsabilidades
- Autenticação segura
- ORM
- CI/CD
- Infra como código
- Automação de serviços

---

## 👨‍💻 Autor

**Iago Rodrigues**  
GitHub: https://github.com/IagoRdgs

---

## 📄 Licença

Licença **MIT** — uso livre 🚀

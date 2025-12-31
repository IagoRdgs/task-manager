# 📝 Task Manager - Full Stack Ecosystem

<p align="center">
  <img src="https://img.shields.io/badge/Status-Concluído-success?style=for-the-badge" alt="Status">
  <img src="https://img.shields.io/badge/Deploy-Vercel-black?style=for-the-badge&logo=vercel" alt="Deploy">
  <img src="https://img.shields.io/badge/Database-Supabase-3ECF8E?style=for-the-badge&logo=supabase" alt="Database">
</p>

O **Task Manager** é uma plataforma robusta de produtividade que gerencia o ciclo de vida completo de tarefas. O projeto foi construído para demonstrar proficiência em operações **CRUD complexas**, autenticação segura e integração de serviços em nuvem.

---

### 📸 Preview do Projeto

<p align="center">
  <img src="https://github.com/IagoRdgs/task-manager/blob/master/frontend/public/image.png" width="100%" alt="Dashboard Preview">
</p>

---

### 🛠️ Stack Tecnológica & Arquitetura

Este projeto utiliza uma arquitetura desacoplada para garantir escalabilidade:

- **Frontend:** [React.js](https://reactjs.org/) + [Bootstrap](https://getbootstrap.com/) (Interface responsiva e limpa)
- **Backend:** [Node.js](https://nodejs.org/) + [Express](https://expressjs.com/) (API RESTful)
- **ORM:** [Prisma](https://www.prisma.io/) (Tipagem forte e queries otimizadas)
- **Database:** [Supabase](https://supabase.com/) (PostgreSQL em nuvem)
- **Segurança:** [JWT](https://jwt.io/) (JSON Web Tokens para sessões seguras)
- **CI/CD:** [GitHub Actions](https://github.com/features/actions) (Automação de infraestrutura)

---

### 📂 Estrutura do Projeto

```text
task-manager/
├── frontend/          # Aplicação React (Frontend)
│   ├── src/
│   │   ├── components/  # Componentes reutilizáveis
│   │   ├── pages/       # Login, Dashboard, Cadastro
│   │   └── api/    # Integração com API (Axios)
├── api/          # API Node.js (Backend)
│   ├── prisma/      # Schema do Banco de Dados
│   ├── src/
│   │   ├── controllers/ # Lógica de negócio
│   │   ├── middleware/  # Filtros de Auth (JWT)
│   │   └── routes/      # Endpoints da API
└── .github/         # Automações (Keep Alive)

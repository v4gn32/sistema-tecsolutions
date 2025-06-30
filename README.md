# 🛠️ TecSolutions Service Manager

Sistema web completo para automação de relatórios técnicos e gestão de atendimentos da empresa TecSolutions. A plataforma visa substituir o uso manual de arquivos Word e pastas no OneDrive por um sistema moderno com dashboards, controle de clientes, tickets, equipamentos, relatórios e muito mais.

---

## 🎯 Objetivo

Automatizar o processo de geração e organização de relatórios técnicos, otimizando o fluxo de trabalho entre técnicos e administradores da TecSolutions.

---

## 🔧 Funcionalidades

- Login com autenticação JWT (admin e técnico)
- Cadastro e gerenciamento de clientes
- Registro de equipamentos por cliente
- Criação de tickets de atendimento
  - Tipo: Presencial, Remoto, Laboratório
  - Registro de materiais e horas técnicas
- Geração automática de relatórios em PDF
- Upload de fotos e anexos
- Filtros por cliente, período, status e tipo de atendimento
- Dashboard com estatísticas e pendências
- Histórico de serviços e envio automático por e-mail
- Controle de usuários e permissões

---

## 🧱 Tecnologias Utilizadas

### Backend
- Node.js
- Express
- Prisma ORM
- PostgreSQL
- JWT para autenticação
- Multer para upload de arquivos

### Frontend
- Angular 20
- Tailwind CSS
- Angular Services + HTTP Client

### DevOps
- Docker e Docker Compose
- Deploy via Render ou Railway (sugestão)

---

## 🚀 Como rodar o projeto localmente

### Pré-requisitos

- Node.js 18+
- Angular CLI
- Docker e Docker Compose

### Passo a passo

1. Clone o repositório:

```bash
git clone https://github.com/v4gn32/sistema-tecsolutions.git
cd sistema-tecsolutions
```

2. Instale as dependências:

```bash
# Backend
cd backend
npm install

# Frontend
cd ../frontend
npm install
```

3. Inicie banco com Docker:

```bash
docker-compose up -d
```

4. Execute as migrações Prisma:

```bash
cd backend
npx prisma migrate dev --name init
```

5. Rode o backend:

```bash
npm run dev
```

6. Rode o frontend:

```bash
cd ../frontend
ng serve
```

7. Acesse:
- Frontend: http://localhost:4200  
- Backend: http://localhost:3000

---

## 📂 Estrutura de Diretórios

```
sistema-tecsolutions/
│
├── backend/               # Backend Node.js + Express
│   ├── src/
│   ├── prisma/
│   └── .env
│
├── frontend/              # Frontend Angular
│   ├── src/
│   └── angular.json
│
├── docker-compose.yml     # PostgreSQL e serviços
└── README.md
```

---

## ✍️ Autor

Desenvolvido por Vagner Oliveira  
🔗 GitHub: [github.com/v4gn32](https://github.com/v4gn32)

---

## 📃 Licença

Este projeto está licenciado sob a Licença MIT.

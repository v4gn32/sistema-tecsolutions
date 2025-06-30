# 💰 VOF Financeiro

Sistema completo de gestão financeira pessoal, com suporte a lançamentos de receitas, despesas, parcelamentos e emissão de notas como MEI. Desenvolvido com Angular, Node.js, PostgreSQL e Docker.

## 📌 Funcionalidades

- Login com senha (usuário comum e administrador)
- Dashboard moderna com cards de resumo
- Lançamento de receitas e despesas
- Cálculo automático de totais
- Controle de parcelamentos
- Registro de notas fiscais emitidas como MEI
- Backend com API RESTful segura (JWT)
- Banco de dados PostgreSQL
- Docker para facilitar deploy e ambiente local

---

## 🧱 Tecnologias Utilizadas

### Frontend
- Angular 20
- Tailwind CSS

### Backend
- Node.js
- Express
- PostgreSQL
- Prisma ORM
- JWT

### DevOps
- Docker + Docker Compose

---

## 🛠️ Como rodar o projeto localmente

### Pré-requisitos

- Node.js 18+
- Docker e Docker Compose
- Angular CLI `npm install -g @angular/cli`

### Passo a passo

1. Clone o repositório:

```bash
git clone https://github.com/v4gn32/vof-financeiro.git
cd vof-financeiro
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

3. Inicie os containers com PostgreSQL:

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
vof-financeiro/
│
├── backend/              # Backend Node.js + Express
│   ├── src/
│   ├── prisma/
│   └── .env
│
├── frontend/             # Frontend Angular
│   ├── src/
│   └── angular.json
│
├── docker-compose.yml    # Orquestração do PostgreSQL
└── README.md
```

---

## ✍️ Autor

Desenvolvido por Vagner Oliveira  
📧 Contato: [seu-email@email.com]  
🔗 GitHub: [github.com/v4gn32](https://github.com/v4gn32)

---

## 📃 Licença

Este projeto está licenciado sob a Licença MIT.

# 📝 Blog Pessoal

Aplicação web full stack de blog pessoal com área pública de leitura e área autenticada para gerenciamento de postagens.

## 🔗 Links

- **Frontend (produção):** https://blog-pessoal-ruddy-five.vercel.app
- **Backend (produção):** https://blogpessoal-013m.onrender.com
- **Documentação da API (Swagger):** https://blogpessoal-013m.onrender.com/swagger

---

## 📌 Sobre o Projeto

O Blog Pessoal é uma plataforma completa de blog que permite a qualquer visitante navegar pelas postagens públicas, e ao usuário autenticado criar, editar e excluir seus próprios conteúdos. O projeto foi desenvolvido com foco em boas práticas de autenticação, integração Front-End/Back-End e deploy em ambiente de produção.

---

## ✨ Funcionalidades

- Cadastro e login de usuários com autenticação via JWT
- Rotas protegidas no frontend para usuários autenticados
- CRUD completo de postagens (criar, listar, editar e excluir)
- Feedback visual de ações com React Toastify
- Layout responsivo
- Documentação da API com Swagger

---

## 🛠️ Tecnologias Utilizadas

### Frontend
| Tecnologia | Descrição |
|---|---|
| React | Biblioteca para construção de interfaces |
| Vite | Build tool e servidor de desenvolvimento |
| TypeScript | Tipagem estática |
| Tailwind CSS | Estilização utilitária |
| Axios | Requisições HTTP |
| React Toastify | Notificações e feedback visual |

### Backend
| Tecnologia | Descrição |
|---|---|
| NestJS | Framework Node.js para o servidor |
| TypeORM | ORM para mapeamento de entidades |
| MySQL | Banco de dados em desenvolvimento |
| PostgreSQL | Banco de dados em produção (Render) |
| JWT | Autenticação e controle de acesso |
| Swagger | Documentação da API |

---

## 🚀 Como Rodar Localmente

### Pré-requisitos

- Node.js (versão 18 ou superior)
- npm ou yarn
- MySQL rodando localmente

### Frontend

```bash
# Clone o repositório
git clone https://github.com/ThaysPei/blog-pessoal.git

# Acesse a pasta do frontend
cd blog-pessoal

# Instale as dependências
npm install

# Inicie o servidor de desenvolvimento
npm run dev
```

A aplicação estará disponível em `http://localhost:5173`.

### Backend

```bash
# Acesse a pasta do backend
cd blog-pessoal-backend

# Instale as dependências
npm install

# Configure as variáveis de ambiente
cp .env.example .env
# Preencha as variáveis no arquivo .env

# Inicie o servidor
npm run start:dev
```

O servidor estará disponível em `http://localhost:3000`.

---

## 🔐 Variáveis de Ambiente

Crie um arquivo `.env` na raiz do backend com as seguintes variáveis:

```env
DB_HOST=localhost
DB_PORT=3306
DB_USERNAME=seu_usuario
DB_PASSWORD=sua_senha
DB_DATABASE=blogpessoal
JWT_SECRET=seu_secret
```

---

## 📁 Estrutura de Pastas (Frontend)

```
src/
├── components/       # Componentes reutilizáveis
├── pages/            # Páginas da aplicação
├── services/         # Configuração do Axios e chamadas à API
├── contexts/         # Contextos de autenticação
├── App.tsx           # Componente raiz e rotas
└── main.tsx          # Ponto de entrada
```

---

## 🌐 Deploy

- **Frontend:** Vercel — deploy contínuo a partir da branch `main`
- **Backend:** Render — banco de dados PostgreSQL em produção
- Variáveis de ambiente configuradas separadamente em cada plataforma, mantendo dados sensíveis fora do código

---

## 👩‍💻 Autora

Desenvolvido por **Thays Peixoto**

[![GitHub](https://img.shields.io/badge/GitHub-ThaysPei-181717?style=flat&logo=github)](https://github.com/ThaysPei)

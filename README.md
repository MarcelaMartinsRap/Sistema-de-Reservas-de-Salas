# 🏢 Sistema de Reservas de Salas de Estudo/Reunião

Projeto desenvolvido no Bootcamp Full Stack com o objetivo de criar uma aplicação web completa para reservas de salas, aplicável a universidades, coworkings, empresas ou bibliotecas.

---

## 📌 Funcionalidades

- Cadastro e login de usuários
- Visualização de salas disponíveis
- Reserva de salas por data e horário
- Edição e cancelamento de reservas
- Histórico pessoal de reservas
- Documentação da API via Swagger

---

## 🛠️ Tecnologias Utilizadas

### Backend
- Node.js
- Express.js
- PostgreSQL (sem ORM, com SQL puro)
- Bcrypt.js (criptografia de senhas)
- Swagger (documentação da API)

### Frontend (em progresso)
- React.js / Next.js

---

## 🔐 Segurança

- Senhas armazenadas com hash utilizando Bcrypt
- Validação de horários para evitar conflitos de reserva
- Campos obrigatórios validados no backend

---

## 📄 Documentação da API

A documentação da API está disponível via Swagger.

Para acessar:
```bash
http://localhost:3000/api-docs

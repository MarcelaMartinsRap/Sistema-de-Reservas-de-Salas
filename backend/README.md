# Backend - Sistema de Reservas de Salas

## Como rodar localmente

1. Instale as dependências:
   ```bash
   cd backend
   npm install
   ```

2. Crie um arquivo `.env` na raiz do backend com as variáveis de ambiente necessárias. Exemplo:
   ```env
   PORT=3000
   DB_HOST=localhost
   DB_PORT=5432
   DB_USER=seu_usuario
   DB_PASSWORD=sua_senha
   DB_NAME=reservas
   DATABASE_URL="postgresql://seu_usuario:sua_senha@localhost:5432/reservas"
   ```
   > **Nunca exponha dados sensíveis (usuário/senha) em repositórios públicos.**

3. Crie o banco de dados no PostgreSQL (se ainda não existir):
   ```bash
   createdb -U seu_usuario -h localhost -p 5432 reservas
   # senha: sua_senha
   ```

4. Para rodar em modo desenvolvimento:
   ```bash
   npx ts-node src/app.ts
   ```
   Ou, se preferir hot reload:
   ```bash
   npx nodemon src/app.ts
   ```

## Estrutura de Pastas

```
backend/
  src/
    controllers/
    dtos/
    middlewares/
    routes/
    services/
    models/
    types/
    utils/
    config/
    app.ts
    redisClient.ts
  .env
  package.json
  tsconfig.json
```

## Observações
- Não há autenticação, queries SQL reais ou regras de negócio implementadas neste setup inicial.
- O projeto está pronto para expansão modular.

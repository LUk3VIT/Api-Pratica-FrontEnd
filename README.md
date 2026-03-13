# Front-Pratica

Interface Web simplificada para consumo da **API-Pratica** (E-commerce). Desenvolvida para realizar a autenticação de usuários e o gerenciamento (CRUD) de produtos via interface gráfica.

### Status
**Protótipo / Funcional** — Pronto para integração local.

### Tecnologias
* **Frontend:** (Ex: HTML estático)
* **Comunicação:** Axios / Fetch API

### Pré-requisitos
* **Node.js** >= 16
* **API-Pratica** rodando em: `http://localhost:3000`

---

### Instalação e Execução

1. **Instale as dependências:**
   ```bash
   npm install
   ```

2. **Suba o servidor local (Via Localhost):**
   ```bash
   npx serve .
   ```

### Integração com a API
O frontend consome os endpoints da API-Pratica utilizando a URL base de localhost.

- URL da API: http://localhost:3000/api
- Persistência: O token recebido no login é armazenado no localStorage.

Endpoints Consumidos:
- Autenticação:

  - POST /auth/register — Cadastro de novo usuário.

  - POST /auth/login — Login e recebimento de Token JWT.

- Produtos (Requer Header Authorization):

  - GET /produto — Listagem geral.

  - POST /produto — Criação de novo item.

  - PUT /produto/:id — Edição de dados.

  - DELETE /produto/:id — Remoção de item.

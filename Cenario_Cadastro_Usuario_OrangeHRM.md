
# ✅ Cenário de Teste – Cadastro de Usuário no OrangeHRM

| **ID**        | CT_RF04 |
|---------------|---------|
| **Requisito** | Cadastro de novo colaborador no sistema OrangeHRM |
| **Módulo**    | PIM - Employee Management |
| **Funcionalidade** | Adicionar novo colaborador |
| **Descrição** | Validar se o sistema permite o cadastro de um novo colaborador com sucesso, preenchendo os campos obrigatórios. |
| **Pré-condição** | Estar logado no sistema OrangeHRM com perfil de Administrador ou RH. |
| **Pós-condição** | Colaborador cadastrado deve estar visível na lista de empregados. |

---

## 🧪 Casos de Teste

### ✔️ Caso 1 - Cadastro de colaborador com dados válidos

| **Etapa** | **Ação**                                                                 |
|-----------|---------------------------------------------------------------------------|
| 1         | Acessar o sistema **OrangeHRM**                                           |
| 2         | Realizar login com credenciais válidas                                    |
| 3         | Navegar até o menu **PIM > Add Employee**                                 |
| 4         | Preencher os campos obrigatórios (First Name, Last Name, Employee ID)     |
| 5         | Clicar no botão **Save**                                                  |
| 6         | Verificar se o sistema redireciona para a página de detalhes do colaborador |

---

### ✔️ Caso 2 - Cadastro com campos obrigatórios em branco

| **Etapa** | **Ação**                                                                 |
|-----------|---------------------------------------------------------------------------|
| 1         | Acessar o sistema **OrangeHRM**                                           |
| 2         | Realizar login com credenciais válidas                                    |
| 3         | Navegar até o menu **PIM > Add Employee**                                 |
| 4         | Deixar os campos obrigatórios em branco                                   |
| 5         | Clicar em **Save**                                                        |
| 6         | Verificar se o sistema exibe mensagens de erro de validação               |

---

### ✔️ Caso 3 - Cadastro com ativação de conta de login

| **Etapa** | **Ação**                                                                 |
|-----------|---------------------------------------------------------------------------|
| 1         | Acessar o sistema **OrangeHRM**                                           |
| 2         | Realizar login com perfil de Administrador                                |
| 3         | Navegar até **PIM > Add Employee**                                        |
| 4         | Preencher os campos obrigatórios e habilitar a opção **Create Login Details** |
| 5         | Preencher login, senha e status da conta                                  |
| 6         | Clicar em **Save**                                                        |
| 7         | Verificar se o usuário foi cadastrado com credenciais de acesso           |

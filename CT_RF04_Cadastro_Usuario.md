
# CT_RF04: Cadastro de Usuário

## CT_RF04_01: Cadastro com dados válidos

**ID:** CT_RF04_01  
**Requisito:** RF04 - Cadastro de usuário  
**Título:** Validar o cadastro de um novo usuário com todos os dados obrigatórios  
**Objetivo:** Verificar se é possível cadastrar um novo colaborador informando apenas os dados obrigatórios  
**Pré-condições:**  
- Usuário autenticado no OrangeHRM  
- Acesso ao menu PIM > Add Employee  

### Passos:

1. Acessar o OrangeHRM  
2. Realizar login com um usuário válido  
3. No menu lateral, clicar em "PIM"  
4. Selecionar “Add Employee”  
5. Preencher os campos obrigatórios:  
   - First Name: Ana  
   - Last Name: Silva  
6. Clicar em "Save"

### Resultado Esperado:
- Usuário é cadastrado com sucesso  
- Sistema redireciona para a tela de detalhes do novo colaborador  

---

## CT_RF04_02: Cadastro com criação de login

**ID:** CT_RF04_02  
**Requisito:** RF04 - Cadastro de usuário  
**Título:** Verificar cadastro com opção de criar login de acesso ao sistema  
**Objetivo:** Garantir que é possível criar login de sistema durante o cadastro do usuário  
**Pré-condições:**  
- Usuário autenticado  
- Acesso ao menu PIM > Add Employee  

### Passos:

1. Acessar o OrangeHRM  
2. Realizar login com um usuário válido  
3. Navegar até "PIM" > "Add Employee"  
4. Preencher os campos obrigatórios (First Name, Last Name)  
5. Habilitar a opção “Create Login Details”  
6. Informar:
   - Username: ana.silva  
   - Password: Senha123!  
   - Confirm Password: Senha123!  
   - Status: Enabled  
7. Clicar em “Save”

### Resultado Esperado:
- Cadastro do colaborador e do usuário de login concluído com sucesso  
- Perfil do colaborador exibido após o salvamento  

---

## CT_RF04_03: Cadastro com campos obrigatórios em branco

**ID:** CT_RF04_03  
**Requisito:** RF04 - Cadastro de usuário  
**Título:** Validar comportamento ao tentar cadastrar sem preencher campos obrigatórios  
**Objetivo:** Garantir que o sistema não permite salvar um cadastro com campos obrigatórios vazios  
**Pré-condições:**  
- Usuário autenticado  
- Acesso ao menu PIM > Add Employee  

### Passos:

1. Acessar o OrangeHRM  
2. Fazer login com usuário válido  
3. Acessar “PIM” > “Add Employee”  
4. Deixar os campos First Name e Last Name vazios  
5. Clicar em "Save"

### Resultado Esperado:
- Sistema deve exibir mensagens de erro indicando campos obrigatórios  
- Cadastro não é salvo  

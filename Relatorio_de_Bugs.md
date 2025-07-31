# Relatório de Bugs  
**Software:** OrangeHRM  

**QA responsável:** Richard Dias  

**Data:** 31/07/2025  

---

### 🐞 Bug 01: Ícone para visualizar senha desaparece ao clicar fora do campo  
**ID:** BUG-001  
**Descrição:**  
O ícone que permite visualizar a senha some quando o usuário clica fora do campo, e não reaparece ao tentar ativá-lo novamente, o que impede o usuário de conferir a senha digitada.  

**Severidade:** Média  
**Prioridade:** Alta  
**Status:** Aberto  

**Passos para reproduzir:**  
1. Acessar a página de login  
2. Digitar a senha no campo destinado  
3. Clicar no ícone para visualizar a senha  
4. Clicar fora do campo de senha  
5. Tentar clicar novamente para visualizar a senha  

**Resultado esperado:**  
O ícone de visualização deve permanecer visível e funcional, mesmo após perder o foco do campo.  

**Resultado obtido:**  
O ícone desaparece e não pode ser ativado novamente, dificultando a visualização da senha.  

**Evidência:** https://jam.dev/c/3e4a0cd8-0b5c-4bc3-86ce-c8300a7801b0

**Ambiente:**  
- Ambiente de homologação  
- Windows 11  
- Microsoft Edge v.136.0  
- OrangeHRM Demo  

**Funcionalidade afetada:** Login / Criação de usuário  
**Caso de teste relacionado:** C01-CT01: Login com e-mail e senha válidos    

---

### 🐞 Bug 02: Página de login atualiza após erro de autenticação  
**ID:** BUG-002  
**Descrição:**  
Ao inserir credenciais incorretas, a página de login é recarregada, o que prejudica a experiência do usuário por não apresentar a mensagem de erro de forma dinâmica.  

**Severidade:** Baixa  
**Prioridade:** Média  
**Status:** Aberto  

**Passos para reproduzir:**  
1. Acessar a página de login  
2. Inserir usuário ou senha inválidos  
3. Clicar no botão “Login”  

**Resultado esperado:**  
Exibir a mensagem de erro sem que a página seja atualizada.  

**Resultado obtido:**  
A página é recarregada antes de mostrar a mensagem de erro.  

**Ambiente:**  
- Ambiente de homologação  
- Windows 11  
- Microsoft Edge v.136.0  
- OrangeHRM Demo  

**Funcionalidade afetada:** Login  
**Caso de teste relacionado:** C01-CT02: Login com credenciais inválidas    

---

### 🐞 Bug 03: Falta de mensagem clara após login com sucesso ou falha  
**ID:** BUG-003  
**Descrição:**  
O sistema não apresenta mensagem clara de sucesso ou erro após o login, apenas redireciona ou atualiza a página, o que pode causar dúvidas no usuário.  

**Severidade:** Média  
**Prioridade:** Média  
**Status:** Aberto  

**Passos para reproduzir:**  
1. Acessar a página de login  
2. Inserir credenciais válidas  
3. Clicar em “Login”  

**Resultado esperado:**  
Exibir mensagem indicando sucesso no login, como “Login realizado com sucesso”.  

**Resultado obtido:**  
Usuário é redirecionado sem receber nenhuma confirmação visual.  

**Ambiente:**  
- Ambiente de homologação  
- Windows 11  
- Microsoft Edge v.136.0  
- OrangeHRM Demo  

**Funcionalidade afetada:** Login  
**Caso de teste relacionado:** C01-CT01: Login com e-mail e senha válidos   

---

### 🐞 Bug 04: Não há opções para aplicar licença de férias  
**ID:** BUG-004  
**Descrição:**  
No módulo de férias, ao tentar aplicar uma licença, não aparecem opções para seleção, e é exibida a mensagem “No Leave Types with Leave Balance”, impedindo a solicitação.  

**Severidade:** Alta  
**Prioridade:** Alta  
**Status:** Aberto  

**Passos para reproduzir:**  
1. Acessar o menu “Leave”  
2. Clicar em “Apply”  
3. Verificar se há opções de licença disponíveis  

**Resultado esperado:**  
Listar os tipos de licença que possuem saldo disponível para uso.  

**Resultado obtido:**  
É exibida apenas a mensagem informando que não há tipos de licença com saldo.  

**Ambiente:**  
- Ambiente de homologação  
- Windows 11  
- Microsoft Edge v.136.0  
- OrangeHRM Demo  

**Funcionalidade afetada:** Férias  
**Caso de teste relacionado:** C04-CT01: Aplicar licença de férias com dados válidos  
 

---

### 🐞 Bug 05: Ícone para visualizar senha desaparece no cadastro de funcionário  
**ID:** BUG-005  
**Descrição:**  
No formulário de cadastro de funcionário no módulo PIM, o ícone para visualizar a senha some ao clicar fora do campo de senha ou confirmação, e não reaparece ao tentar novamente.  

**Severidade:** Média  
**Prioridade:** Alta  
**Status:** Aberto  

**Passos para reproduzir:**  
1. Navegar até o módulo “PIM”  
2. Clicar em “Add Employee”  
3. Marcar “Create Login Details”  
4. Clicar no ícone para visualizar a senha  
5. Clicar fora do campo e tentar ativar o ícone novamente  

**Resultado esperado:**  
O ícone deve permanecer visível e funcionar mesmo após sair do campo.  

**Resultado obtido:**  
O ícone desaparece e não pode ser acionado novamente.  

**Ambiente:**  
- Ambiente de homologação  
- Windows 11  
- Microsoft Edge v.136.0  
- OrangeHRM Demo  

**Funcionalidade afetada:** Cadastro de funcionário  
**Caso de teste relacionado:** C03-CT01: Criar novo funcionário com dados válidos   

---

### 🐞 Bug 06: Erro ao tentar reagendar entrevista já agendada  
**ID:** BUG-006  
**Descrição:**  
No módulo de Recrutamento, ao tentar reagendar ou visualizar uma entrevista já marcada, ocorre um erro que impede o carregamento dos detalhes da entrevista.  

**Severidade:** Alta  
**Prioridade:** Alta  
**Status:** Aberto  

**Passos para reproduzir:**  
1. Acessar o módulo “Recruitment”  
2. Abrir perfil de candidato  
3. Identificar entrevista já agendada  
4. Tentar reagendar ou visualizar detalhes  
5. Observar o erro apresentado  

**Resultado esperado:**  
As informações da entrevista devem ser carregadas corretamente.  

**Resultado obtido:**  
O sistema apresenta erro e não permite a ação desejada.  

**Ambiente:**  
- Ambiente de homologação  
- Windows 11  
- Microsoft Edge v.136.0  
- OrangeHRM Demo  

**Funcionalidade afetada:** Recrutamento  
**Caso de teste relacionado:** C05-CT03: Buscar e interagir com candidatos existentes    

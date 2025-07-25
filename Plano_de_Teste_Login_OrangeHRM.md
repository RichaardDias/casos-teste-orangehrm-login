
# Plano de Teste Funcional – Login na Plataforma OrangeHRM

| **ID**      | **Título do Caso de Teste**                          | **Pré-condições**                               | **Passos**                                                                 | **Resultado Esperado**                                   | **Status** |
|-------------|------------------------------------------------------|--------------------------------------------------|---------------------------------------------------------------------------|-----------------------------------------------------------|------------|
| CT_RF01_01  | Login com credenciais válidas                        | Estar na página de login                         | 1. Digitar usuário válido<br>2. Digitar senha válida<br>3. Clicar em "Login" | Usuário é redirecionado para o dashboard                  | ✅ Aprovado |
| CT_RF01_02  | Login com senha incorreta                            | Estar na página de login                         | 1. Digitar usuário válido<br>2. Digitar senha inválida<br>3. Clicar em "Login" | Mensagem de erro é exibida: "Invalid credentials"         | ✅ Aprovado |
| CT_RF01_03  | Login com campos em branco                           | Estar na página de login                         | 1. Deixar usuário e senha em branco<br>2. Clicar em "Login"                | Mensagem de erro nos campos obrigatórios                  | ✅ Aprovado |
| CT_RF01_04  | Login com usuário inexistente                        | Estar na página de login                         | 1. Digitar usuário inexistente<br>2. Digitar qualquer senha<br>3. Clicar em "Login" | Mensagem de erro: "Invalid credentials"                  | ✅ Aprovado |
| CT_RF01_05  | Verificar campo de senha com caracteres especiais    | Estar na página de login                         | 1. Digitar senha com símbolos especiais<br>2. Clicar em "Login"            | Plataforma aceita os caracteres e retorna resposta adequada | ✅ Aprovado |

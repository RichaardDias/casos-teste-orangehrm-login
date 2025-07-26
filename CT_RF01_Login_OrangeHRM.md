# Casos de Teste - OrangeHRM (Login)

Sistema: OrangeHRM  
Módulo: Autenticação / Login  
Tipo de Teste: Funcional Manual  

| ID         | Título                                           | Pré-condições                              | Passos                                                                                      | Resultado Esperado                                                                 |
|------------|--------------------------------------------------|--------------------------------------------|---------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------|
| CT_RF01_01 | Login com credenciais válidas                    | Usuário cadastrado com login e senha válidos | 1. Acessar o sistema OrangeHRM<br>2. Preencher campo "Username" com usuário válido<br>3. Preencher campo "Password" com senha válida<br>4. Clicar em "Login"             | Usuário autenticado e redirecionado para o dashboard principal do sistema         |
| CT_RF01_02 | Login com senha incorreta                        | Usuário cadastrado no sistema               | 1. Acessar o sistema OrangeHRM<br>2. Preencher campo "Username" com usuário válido<br>3. Preencher campo "Password" com senha inválida<br>4. Clicar em "Login"           | Sistema exibe mensagem de erro: "Invalid credentials"                              |
| CT_RF01_03 | Tentativa de login com campos em branco          | Nenhuma                                     | 1. Acessar o sistema OrangeHRM<br>2. Deixar campos "Username" e "Password" em branco<br>3. Clicar em "Login"                                                           | Sistema exibe mensagens de validação obrigatória nos campos                        |

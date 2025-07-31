# Plano de Testes Funcionais – OrangeHRM

## 1. Login na Plataforma

| ID       | Caso de Teste                                      | Entrada                           | Resultado Esperado                                    | Prioridade |
|----------|----------------------------------------------------|-----------------------------------|--------------------------------------------------------|------------|
| CT_RF01_01 | Login com credenciais válidas                    | Usuário: Admin / Senha: admin123  | Redirecionamento para o dashboard                      | Alta       |
| CT_RF01_02 | Login com senha incorreta                        | Usuário: Admin / Senha: errada    | Mensagem de erro “Invalid credentials”                 | Alta       |
| CT_RF01_03 | Login com campos em branco                       | Usuário: (vazio) / Senha: (vazio) | Alerta de campos obrigatórios                          | Média      |

## 2. Acesso e Visualização do Dashboard

| ID       | Caso de Teste                                       | Entrada         | Resultado Esperado                                       | Prioridade |
|----------|-----------------------------------------------------|-----------------|-----------------------------------------------------------|------------|
| CT_RF02_01 | Acesso ao dashboard após login                    | Login realizado | Visualização dos cards do painel                         | Alta       |
| CT_RF02_02 | Verificação de indicadores visíveis               | Login realizado | Exibição de elementos como "Time at Work", "Leave", etc. | Média      |
| CT_RF02_03 | Verificar resposta do sistema a falha de carregamento | Erro no backend | Mensagem de erro amigável ou fallback                    | Média      |

## 3. Gestão de Funcionários (Módulo PIM)

| ID       | Caso de Teste                                   | Entrada                          | Resultado Esperado                                   | Prioridade |
|----------|-------------------------------------------------|----------------------------------|-------------------------------------------------------|------------|
| CT_RF03_01 | Cadastro de novo funcionário                  | Dados completos de funcionário   | Funcionário listado no PIM                           | Alta       |
| CT_RF03_02 | Edição de dados de funcionário existente       | Alterar endereço ou cargo        | Dados atualizados com sucesso                        | Alta       |
| CT_RF03_03 | Pesquisa de funcionário pelo nome              | Nome do funcionário              | Exibição do resultado correto                        | Média      |

## 4. Solicitação e Gerenciamento de Férias

| ID       | Caso de Teste                                  | Entrada                      | Resultado Esperado                                   | Prioridade |
|----------|------------------------------------------------|------------------------------|-------------------------------------------------------|------------|
| CT_RF04_01 | Solicitação de férias                        | Data início e fim válidas    | Férias solicitadas com sucesso                       | Alta       |
| CT_RF04_02 | Tentativa de solicitar férias em datas inválidas | Data fim anterior à início | Mensagem de erro e bloqueio da ação                  | Alta       |
| CT_RF04_03 | Aprovação de férias pelo gestor              | Seleção de solicitação       | Solicitação aprovada e refletida no sistema          | Média      |

## 5. Gerenciamento de Candidatos (Recrutamento)

| ID       | Caso de Teste                                  | Entrada                          | Resultado Esperado                                   | Prioridade |
|----------|------------------------------------------------|----------------------------------|-------------------------------------------------------|------------|
| CT_RF05_01 | Cadastro de novo candidato                   | Dados do currículo               | Candidato adicionado na lista                        | Alta       |
| CT_RF05_02 | Alterar status do processo seletivo           | Selecionar status “Entrevista”   | Atualização registrada no sistema                    | Média      |
| CT_RF05_03 | Pesquisa por candidato específico             | Nome completo                    | Exibição correta do candidato                        | Média      |

## 6. Gerenciamento de Usuários (Administração)

| ID       | Caso de Teste                                | Entrada                           | Resultado Esperado                                   | Prioridade |
|----------|----------------------------------------------|-----------------------------------|-------------------------------------------------------|------------|
| CT_RF06_01 | Adição de novo usuário                     | Login, nome e papel               | Usuário criado e listado                             | Alta       |
| CT_RF06_02 | Desativação de usuário                      | Selecionar usuário → “Disable”    | Status atualizado para “Disabled”                    | Alta       |
| CT_RF06_03 | Filtragem por papel ou status               | Filtros no Admin                  | Lista atualizada conforme critérios                  | Média      |

## 7. Registro de Ponto (Controle de Horas)

| ID       | Caso de Teste                                   | Entrada                      | Resultado Esperado                                   | Prioridade |
|----------|-------------------------------------------------|------------------------------|-------------------------------------------------------|------------|
| CT_RF07_01 | Registrar entrada de trabalho                 | Hora de entrada válida       | Registro salvo no sistema                            | Alta       |
| CT_RF07_02 | Registrar saída sem entrada prévia            | Apenas hora de saída         | Mensagem de erro “Entrada não registrada”            | Alta       |
| CT_RF07_03 | Visualizar histórico de marcações             | Selecionar intervalo de datas| Exibição das marcações feitas                        | Média      |

## 8. Relatórios do Sistema

| ID       | Caso de Teste                                 | Entrada                              | Resultado Esperado                                   | Prioridade |
|----------|-----------------------------------------------|--------------------------------------|-------------------------------------------------------|------------|
| CT_RF08_01 | Geração de relatório de presença            | Filtro por período e funcionário     | Relatório gerado com dados precisos                  | Média      |
| CT_RF08_02 | Exportação de relatório para PDF            | Relatório visualizado                | Download do arquivo em formato PDF                   | Média      |
| CT_RF08_03 | Verificação de campos no relatório          | Visualização                         | Campos obrigatórios visíveis                         | Média      |

## 9. Consulta de Colaboradores (Diretório)

| ID       | Caso de Teste                                 | Entrada                      | Resultado Esperado                                   | Prioridade |
|----------|-----------------------------------------------|------------------------------|-------------------------------------------------------|------------|
| CT_RF09_01 | Acesso ao módulo Diretório                  | Login com permissão          | Lista de colaboradores visível                       | Média      |
| CT_RF09_02 | Busca por colaborador                       | Nome completo                | Colaborador correspondente encontrado                | Média      |
| CT_RF09_03 | Verificação de detalhes                     | Clique em colaborador        | Exibição dos dados completos                         | Média      |

## 10. Funcionalidades de Manutenção do Sistema

| ID       | Caso de Teste                                | Entrada                      | Resultado Esperado                                   | Prioridade |
|----------|----------------------------------------------|------------------------------|-------------------------------------------------------|------------|
| CT_RF10_01 | Acesso à tela de manutenção                | Login de admin               | Acesso ao menu de manutenção                         | Média      |
| CT_RF10_02 | Visualização de logs ou backups            | Seleção da funcionalidade    | Listagem correta dos registros                       | Média      |
| CT_RF10_03 | Erro ao tentar excluir item protegido      | Tentativa de exclusão        | Mensagem de erro e bloqueio da operação              | Alta       |

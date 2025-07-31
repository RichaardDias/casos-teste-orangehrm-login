
# ✅ Plano de Testes – OrangeHRM

## 📌 Funcionalidade
Sistema de gestão de RH com funcionalidades como login, controle de ponto, gestão de férias, cadastro de colaboradores, entre outros.

---

## 🎯 Objetivo
Garantir que todas as funcionalidades descritas no escopo estejam operando corretamente por meio de testes manuais baseados em requisitos funcionais.

---

## 🧪 Escopo do Teste

**Módulos testados:**
- Login
- Dashboard
- Gestão de Funcionários (PIM)
- Férias
- Recrutamento
- Administração de Usuários
- Registro de Ponto
- Relatórios
- Diretório
- Manutenção

---

## ⚙️ Ambiente de Testes

- **Ambiente:** Homologação (demo)
- **URL:** [https://opensource-demo.orangehrmlive.com](https://opensource-demo.orangehrmlive.com)
- **Navegadores:** Chrome, Firefox, Edge
- **Plataforma:** Web (Desktop)
- **Acesso:** Usuário: Admin / Senha: admin123

---

## ✅ Critérios de Aceitação

- Todos os testes executados com sucesso.
- Nenhum bug crítico em aberto.
- Interface estável e funcional.
- Validações, mensagens e fluxos corretos.

---

## 🚫 Critérios de Saída

- Casos de teste com status “Pass”.
- Bugs de alta prioridade resolvidos e revalidados.
- Aprovação da equipe de QA.

---

## ⏱️ Técnicas de Teste

- Caixa preta (Black-box)
- Teste funcional
- Teste exploratório
- Teste de regressão manual

---

## 📄 Casos de Teste por Módulo (resumo)

| ID          | Módulo                    | Caso de Teste                                | Prioridade |
|-------------|---------------------------|----------------------------------------------|------------|
| CT_RF01_01  | Login                     | Login com credenciais válidas                | Alta       |
| CT_RF01_02  | Login                     | Login com senha incorreta                    | Alta       |
| CT_RF01_03  | Login                     | Login com campos vazios                      | Média      |
| CT_RF02_01  | Dashboard                 | Acesso ao dashboard após login               | Alta       |
| CT_RF03_01  | Gestão Funcionários (PIM) | Cadastro de novo funcionário                 | Alta       |
| CT_RF04_01  | Férias                    | Solicitação de férias com datas válidas      | Alta       |
| CT_RF05_01  | Recrutamento              | Cadastro de novo candidato                   | Alta       |
| CT_RF06_01  | Administração             | Adição de novo usuário                       | Alta       |
| CT_RF07_01  | Registro de Ponto         | Registrar entrada de trabalho                | Alta       |
| CT_RF08_01  | Relatórios                | Geração de relatório de presença             | Média      |
| CT_RF09_01  | Diretório                 | Acesso ao módulo Diretório                   | Média      |
| CT_RF10_01  | Manutenção                | Acesso à tela de manutenção                  | Média      |

> ℹ️ Casos adicionais estão descritos em detalhes no plano de testes funcional enviado.


## 👥 Responsáveis

| Nome           | Papel       |
|----------------|-------------|
| QA Richard Dias    | Execução  |
|Data: 31/07/2025 |

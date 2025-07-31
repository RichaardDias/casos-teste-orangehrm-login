# 🧪 Relatório Final de Execução de Testes – OrangeHRM Demo

**Responsável:** Richard Dias  
**Data de Execução:** 31/07/2025  
**Tipo de Teste:** Manual  
**Ferramenta testada:** [OrangeHRM Demo](https://opensource-demo.orangehrmlive.com/)  
**Ambiente de Testes:**  
- Sistema Operacional: Windows 11  
- Navegador: Microsoft Edge v.136.0  
- Resolução: 1920x1080  
- Ambiente: Homologação  

---

## ✅ Resumo Geral

| Total de Casos de Teste | Aprovados | Reprovados | Bugs Identificados |
|-------------------------|-----------|------------|---------------------|
| 30                      | 24        | 6          | 6                   |

---

## 📋 Distribuição por Funcionalidade

| Funcionalidade               | Casos Testados | Aprovados | Reprovados |
|-----------------------------|----------------|-----------|------------|
| Login                       | 3              | 1         | 2          |
| Validação de Campos         | 3              | 3         | 0          |
| Cadastro de Funcionário     | 3              | 2         | 1          |
| Aplicar Licença (Férias)    | 3              | 2         | 1          |
| Recrutamento                | 3              | 2         | 1          |
| Menu Administrativo         | 3              | 3         | 0          |
| Time (PIM)                  | 3              | 3         | 0          |
| Dashboard                   | 3              | 3         | 0          |
| Logout                      | 3              | 3         | 0          |
| Navegação Geral             | 3              | 2         | 1          |

---

## 🐞 Bugs Encontrados

| ID       | Título                                                                 | Severidade | Prioridade | Status  |
|----------|------------------------------------------------------------------------|------------|------------|---------|
| BUG-001  | Ícone de visualizar senha desaparece após sair do campo (login)       | Média      | Alta       | Aberto  |
| BUG-002  | Página de login é atualizada após erro de autenticação                 | Baixa      | Média      | Aberto  |
| BUG-003  | Login bem-sucedido sem feedback visual ao usuário                      | Média      | Média      | Aberto  |
| BUG-004  | Nenhum tipo de licença disponível ao aplicar férias                    | Alta       | Alta       | Aberto  |
| BUG-005  | Ícone “ver senha” some no formulário de criação de funcionário         | Média      | Alta       | Aberto  |
| BUG-006  | Falha ao tentar acessar entrevista já agendada (Recrutamento)         | Alta       | Alta       | Aberto  |

---

## 📌 Conclusões

Os testes manuais abrangeram 10 áreas funcionais do sistema OrangeHRM, totalizando 30 casos de teste. A maioria teve sucesso, mas 6 cenários apresentaram falhas e resultaram em bugs reportados. A aplicação demonstrou estabilidade geral, mas requer melhorias em usabilidade, feedback ao usuário e consistência visual de ícones.

---

## ✅ Recomendações

- Adicionar mensagens claras de sucesso/erro no login e cadastro.
- Corrigir o desaparecimento de ícones funcionais (como “ver senha”).
- Verificar e liberar corretamente os tipos de licença no módulo de férias.
- Ajustar o carregamento de entrevistas agendadas no recrutamento.

---

_Em constante aprendizado. Relatório desenvolvido como exercício prático de testes manuais._

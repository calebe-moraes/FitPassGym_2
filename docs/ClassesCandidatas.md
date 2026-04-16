# 📋 Especificação de Requisitos Funcionais

Este documento descreve as funcionalidades do sistema de gestão de academia, organizadas por módulos de operação.

---

## 🛠️ Gestão de Alunos e Planos

| ID | Requisito | Descrição |
| :--- | :--- | :--- |
| **RF01** | **Cadastro de Alunos** | O sistema deve permitir cadastrar novos **alunos** contendo dados pessoais, contato, endereço e plano contratado. |
| **RF02** | **Gerenciamento de Planos** | O sistema deve permitir criar, editar, ativar e desativar tipos de ***planos*** (mensal, trimestral, anual, musculação, funcional etc.). |

---

## 💰 Financeiro e Controle de Acesso

### **RF03 — Controle de Pagamentos**
O sistema deve registrar **pagamentos** realizados na recepção (**dinheiro, cartão ou PIX**) e gerar boletos/cartões para pagamentos online.

### **RF04 — Regularidade do Aluno**
O sistema deve verificar automaticamente se o aluno está com a mensalidade em dia para fins de liberação de serviços.

### **RF05 — Controle de Acesso**
O sistema deve se integrar à **catraca física** para validar a entrada do aluno via tecnologia **RFID**.

---

## 📅 Rotina de Aulas e Avaliações

* **RF06 — Agendamento de Aulas:** O aluno deve poder visualizar horários e reservar vagas nas aulas disponíveis através do sistema.
* **RF07 — Lista de Presença:** Interface para instrutores registrarem a presença dos alunos nas aulas agendadas.
* **RF08 — Avaliação Física:** Registro de métricas como peso, IMC, percentual de gordura e campo para anexar arquivos externos.

---

## 📊 Inteligência de Negócio e Notificações

### **RF09 — Relatórios Gerenciais**
O sistema deve consolidar dados para a emissão de relatórios de:
* 🔴 Inadimplência
* 🟢 Alunos ativos
* 🕒 Histórico de acessos
* 📈 Ocupação das aulas

### **RF10 — Notificações Automáticas**
Envio de alertas ao aluno sobre:
1. Vencimento de mensalidade.
2. Confirmação de agendamento de vaga.
3. Disponibilidade de nova avaliação física.

---

# 🏋️ Sistema de Gestão de Academia

## 📝 Requisitos Funcionais

| ID | Nome | Descrição |
| :--- | :--- | :--- |
| **RF01** | Cadastro de Alunos | Cadastrar alunos com dados pessoais, contato, endereço e plano. |
| **RF02** | Gerenciamento de Planos | Criar, editar, ativar e desativar tipos de planos. |
| **RF03** | Controle de Pagamentos | Registrar pagamentos (Dinheiro/Cartão/PIX) e gerar boletos. |
| **RF04** | Regularidade do Aluno | Verificação automática de status financeiro. |
| **RF05** | Controle de Acesso | Integração com catraca via RFID. |
| **RF06** | Agendamento de Aulas | Visualização de horários e reserva de vagas pelo aluno. |
| **RF07** | Lista de Presença | Registro de presença realizado pelos instrutores. |
| **RF08** | Avaliação Física | Registro de peso, IMC, % de gordura e anexos. |
| **RF09** | Relatórios Gerenciais | Inadimplência, alunos ativos, acessos e ocupação. |
| **RF10** | Notificações | Alertas de vencimento, agendamento e novas avaliações. |

---

## 🗄️ Estrutura de Classes (Atributos)

### 👥 Perfis e Usuários
- **Aluno** (RF01, RF04, RF05, RF06, RF10): `idAluno, nome, cpf, email, telefone, endereco, rfid, status`
- **Instrutor** (RF07, RF08): `idInstrutor, nome, especialidade`
- **Recepcionista** (RF01, RF03): `idRecepcionista, nome`
- **Gerente** (RF02, RF09): `idGerente, nome`

### 💳 Administrativo e Financeiro
- **Plano** (RF01, RF02, RF04): `idPlano, nome, tipo, valor, ativo`
- **Pagamento** (RF03, RF04, RF09): `idPagamento, data, valor, formaPagamento, status`
- **Notificacao** (RF10): `idNotificacao, tipo, dataEnvio, status, mensagem`

### 🏃 Operacional e Aulas
- **Aula** (RF06, RF07, RF09): `idAula, nome, horario, capacidadeMaxima`
- **Agendamento** (RF06, RF10): `idAgendamento, dataReserva, status

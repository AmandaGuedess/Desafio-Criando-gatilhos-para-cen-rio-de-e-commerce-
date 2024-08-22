# Triggers para Cenário de E-commerce

Este projeto demonstra a criação de triggers no banco de dados company, para gerenciar operações de remoção e atualização em um sistema de e-commerce.

## Triggers Criados

### Trigger before_delete_cliente:

- Descrição: Preserva as informações de clientes que excluíram suas contas em uma tabela de histórico (HistoricoCliente).
- Tabela Afetada: Cliente.
- Tabela de Histórico: HistoricoCliente.
  
### Trigger before_update_salario:

- Descrição: Armazena o salário antigo dos colaboradores antes de qualquer atualização de salário, mantendo um histórico de alterações na tabela HistoricoSalario.
- Tabela Afetada: Colaborador.
- Tabela de Histórico: HistoricoSalario.
  
## Como Utilizar

### Para Remoção:

- Ao deletar um cliente da tabela Cliente, os dados são automaticamente copiados para a tabela HistoricoCliente.
  
### Para Atualização:

- Ao atualizar o salário de um colaborador na tabela Colaborador, o salário antigo é armazenado na tabela HistoricoSalario.

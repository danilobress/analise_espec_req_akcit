# Histórias de Usuário - Equipe Financeira

## US10: Validação de Pagamentos para Liberação (Ref: RF10, RN03)
**Como** membro da equipe financeira
**Quero** validar os pagamentos de eventos cobrados antes de liberar definitivamente a vaga do participante
**Para** garantir o recebimento e não ceder vagas para inadimplentes.

### Critérios de Aceitação (BDD)

*   **Cenário 1: Confirmação de inscrição paga**
    *   **Dado** que uma inscrição para evento pago está com status "Aguardando Pagamento"
    *   **Quando** o sistema registrar o recebimento do valor
    *   **Então** a inscrição deve mudar para o status "Confirmada", ocupando a vaga em definitivo, e o participante deve ter acesso ao comprovante.

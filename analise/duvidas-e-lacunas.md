# Dúvidas, Lacunas e Ambiguidades

Para evitar a alucinação e suposições no desenvolvimento, o documento de elicitação aponta áreas críticas onde a informação está incompleta ou conflituosa. Estes pontos devem ser alinhados junto aos stakeholders.

## 1. Inconsistências e Conflitos de Regras
*   **Conflito de Horários de Participantes:** Os organizadores afirmam que os workshops podem ser simultâneos, e os participantes querem se inscrever em vários no mesmo dia. **Dúvida:** O sistema deve barrar o participante se ele tentar se inscrever em dois workshops no exato mesmo horário? Ou apenas exibir um alerta permitindo a inscrição dupla?

## 2. Lacunas de Informação (Necessitam Definição)
*   **Cancelamento (Prazos):** Qual é a antecedência mínima para um participante poder cancelar sua inscrição (ex: até 48h antes do evento)?
*   **Política de Reembolso:** Quais as regras exatas para devolução do dinheiro? Haverá retenção de taxa administrativa?
*   **Comportamento da Lista de Espera:** Como funciona a fila? A convocação é automática se alguém desistir? Qual o prazo para o usuário da lista de espera aceitar a vaga antes de passar para o próximo?
*   **Emissão de Certificados:** O certificado é liberado para todos os inscritos ou o sistema exigirá que a organização faça um controle de "check-in/presença" primeiro?
*   **Comunicações do Sistema:** Por qual canal os comprovantes e notificações serão enviados? (E-mail, SMS, WhatsApp?)
*   **Reserva de Vaga no Checkout:** Quando o usuário clica em "pagar" (ex: boleto gerado), a vaga já sai do estoque ou só sai do estoque quando o banco confirmar (correndo risco de overbooking)?
*   **Privacidade dos Participantes:** Quais informações exatas os palestrantes poderão visualizar? (Nome completo? E-mail? Empresa?)
*   **Métodos e Integração de Pagamento:** Quais serão as formas de pagamento aceitas (PIX, Boleto, Cartão de Crédito)? O sistema utilizará algum gateway de pagamento externo (ex: Stripe, Mercado Pago, Pagar.me) para aprovação automática ou a conciliação será feita manualmente pela equipe financeira?
*   **Transferência de Titularidade (Ticket):** Se o participante não puder comparecer a um evento pago, ele é obrigado a cancelar (e pedir reembolso), ou existe a possibilidade de transferir a sua inscrição para outra pessoa?
*   **Modalidade do Evento (Presencial vs. Online):** A elicitação não detalha o formato físico ou virtual. Se presencial, o sistema gerará QR Codes/Tickets para controle na portaria? Se online, haverá integração com plataformas de videoconferência (Zoom, Teams)?
*   **Inscrições em Lote (B2B / Corporativo):** O sistema deve permitir que uma empresa ou representante compre múltiplas vagas de uma única vez (em um mesmo pedido/pagamento), ou cada participante deverá fazer sua inscrição individualmente (B2C)?
*   **Cupons de Desconto e Lotes:** Haverá necessidade de suporte a códigos promocionais? Os eventos pagos terão controle de precificação dinâmica (ex: Virada de Lote 1 para Lote 2)?
*   **Autenticação e Cadastro (Login):** Como será realizado o acesso ao sistema? Exigirá criação de conta completa (e-mail e senha) antes da inscrição, ou será permitido o uso de Social Login (Google, LinkedIn) ou "checkout como convidado"?

## 3. Requisitos Não Funcionais Críticos a Mapear
*   Definir regras de **LGPD**, **Segurança de Acesso**, **Disponibilidade**, **Desempenho** e **Acessibilidade** com a equipe de TI.

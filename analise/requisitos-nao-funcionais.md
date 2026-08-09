# Requisitos Não Funcionais

A análise do documento de elicitação aponta para a ausência explícita de vários requisitos não funcionais. No entanto, é possível extrair e inferir alguns atributos de qualidade essenciais com base no escopo do projeto e nas necessidades identificadas:

*   **RNF01 (Desempenho e Concorrência):** Como há controle automático de vagas e múltiplos inscritos simultâneos, o sistema deve garantir a consistência dos dados de reserva sob concorrência (evitar overbooking).
*   **RNF02 (Integração e Comunicação):** O sistema deve ser capaz de disparar o envio de comprovantes de inscrição de forma automatizada e com baixa latência após a ação do usuário.
*   **RNF03 (Interface/Usabilidade - Implícito):** O sistema deve centralizar e exibir os eventos em uma interface unificada, simples o suficiente para evitar que o participante precise de ajuda da organização.

### ⚠️ Requisitos Não Funcionais Pendentes (Lacuna)
A seção 4 do documento de elicitação destaca claramente que devem ser definidos atributos técnicos vitais em reuniões futuras:
*   **Segurança e Privacidade (LGPD):** Regras de criptografia, acesso e armazenamento dos dados dos inscritos.
*   **Disponibilidade:** SLAs de uptime (tempo no ar) durante picos de inscrições.
*   **Acessibilidade:** Padrões de acesso para participantes com necessidades especiais (WCAG, etc).
*   **Desempenho Geral:** Tempo de resposta da aplicação e volume de acessos simultâneos suportados.

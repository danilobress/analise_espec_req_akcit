# Glossário de Termos (Linguagem Ubíqua)

Este documento centraliza as definições dos termos de negócio utilizados no **Sistema de Gestão de Eventos**. O objetivo é garantir que a equipe de desenvolvimento, operações e stakeholders utilizem exatamente a mesma nomenclatura, evitando falhas de interpretação sistêmica.

## 1. Atores do Sistema

*   **Participante:** Pessoa interessada em frequentar as programações. Possui permissões para visualizar o catálogo, realizar inscrições, efetuar pagamentos, emitir certificados e solicitar o cancelamento de sua própria vaga.
*   **Organizador:** Membro da empresa (Eventus) responsável pelo *backoffice*. Tem permissão para criar programações, parametrizar regras (vagas, valores, permissão de cancelamento) e monitorar adesões via *dashboard* em tempo real (Nota: O escopo exato destas permissões de parametrização é provisório e será validado posteriormente através de uma Matriz de Acesso oficial com os key users).
*   **Palestrante:** Profissional convidado para ministrar uma atividade específica. Possui acesso restrito apenas para visualização da lista de participantes com inscrição confirmada em suas próprias atividades.
*   **Equipe Financeira:** Setor administrativo responsável por confirmar liquidações de pagamentos, autorizar a transição de inscrições para o status de confirmadas (quando aplicável) e tratar pendências de reembolsos.

## 2. Entidades Sistêmicas (Conceitos Fechados)

*   **Inscrição:** O ato sistêmico do Participante manifestar/comprar sua participação. Trata-se de uma entidade com ciclo de vida (status variando entre: Pendente, Confirmada, Em Espera, Cancelada).
*   **Lista de Espera:** Fila de interessados gerada e populada automaticamente pelo sistema quando o estoque de Vagas de uma atividade é esgotado.
*   **Vaga:** Unidade de disponibilidade consumível. Seu controle dita o limite de superlotação do evento.
*   **Certificado:** Documento de comprovação emitido após o término do evento (Nota: regra de amarração com presença física consta como lacuna a definir).
*   **Comprovante:** Documento transacional disparado imediatamente após a confirmação da inscrição (seja gratuita ou paga).

---

## 3. Termos com Alerta de Ambiguidade de Negócio ⚠️
*Os termos abaixo foram usados como sinônimos durante as entrevistas. Eles exigem um alinhamento com a equipe da Eventus para padronizar as regras e o funcionamento das telas.*

*   **[ALERTA] Evento vs. Workshop:**
    *   *Uso atual no documento:* "Empresa organiza congressos, workshops e eventos... participante quer visualizar todos os eventos... participante quer se inscrever em vários workshops no mesmo dia."
    *   *Decisão de Negócio Pendente:* O sistema deve tratar **Evento** como um guarda-chuva/projeto maior (Ex: "Congresso Nacional") e os **Workshops** como atividades subordinadas dentro deste congresso? Ou, na prática, todos serão cadastrados de forma independente e genérica na mesma lista do catálogo?
*   **[ALERTA] Cancelamento vs. Reembolso:**
    *   *Uso atual no documento:* "Nem todos os eventos permitem cancelamento" vs "Em alguns casos o participante tem direito a reembolso".
    *   *Decisão de Negócio Pendente:* Cancelar a vaga e devolver o dinheiro são regras distintas. Precisamos deixar claro que a ação de **Cancelar** (liberar a vaga de volta para a fila de espera) pode acontecer sem necessariamente gerar um **Reembolso** financeiro. O vocabulário atual mistura as duas operações.

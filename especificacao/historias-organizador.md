# Histórias de Usuário - Organizador

## US06: Controle Automático de Vagas (Ref: RF06)
**Como** organizador
**Quero** que o sistema controle automaticamente a quantidade de vagas disponíveis
**Para** evitar superlotação (*overbooking*).

### Critérios de Aceitação (BDD)

*   **Cenário 1: Vaga disponível consumida**
    *   **Dado** que um evento tem limite de 50 vagas e 49 inscritos confirmados
    *   **Quando** um novo participante efetivar a inscrição
    *   **Então** o estoque de vagas deve ir para 0 e o status do evento deve ser alterado para "Esgotado".

*   **Cenário 2: Bloqueio de inscrição sem vaga**
    *   **Dado** que um evento está com 0 vagas disponíveis ("Esgotado")
    *   **Quando** um usuário visualizar o evento
    *   **Então** o botão de inscrição deve estar bloqueado, sendo oferecida a entrada na lista de espera.

## US07: Lista de Espera Automática (Ref: RF07)
**Como** organizador
**Quero** disponibilizar uma lista de espera quando as vagas de um evento acabarem
**Para** não perder o interesse do público caso ocorram desistências de outros.

### Critérios de Aceitação (BDD)

*   **Cenário 1: Entrada na lista**
    *   **Dado** que o evento está esgotado
    *   **Quando** um participante clicar em "Entrar na fila de espera"
    *   **Então** ele deve ser adicionado à lista aguardando liberação, recebendo um protocolo com data/hora.

## US08: Dashboard em Tempo Real (Ref: RF08)
**Como** organizador
**Quero** visualizar um painel (*dashboard*) com a quantidade de inscritos em tempo real
**Para** acompanhar o engajamento e tomar decisões gerenciais rapidamente.

### Critérios de Aceitação (BDD)

*   **Cenário 1: Atualização dinâmica**
    *   **Dado** que estou com o painel de organizador aberto
    *   **Quando** novas inscrições forem concluídas no sistema
    *   **Então** os contadores de inscritos e vagas devem refletir os dados atualizados em tempo real.

## US09: Configuração de Regras do Evento (Ref: RF09, RF12)
**Como** organizador
**Quero** poder configurar regras específicas de gratuidade e cancelamento ao criar um evento
**Para** adequar o sistema à política variável de cada atividade oferecida.

### Critérios de Aceitação (BDD)

*   **Cenário 1: Evento com restrições**
    *   **Dado** que estou na tela de criação de um novo evento
    *   **Quando** eu configurar o evento como "Pago" e desmarcar a flag "Permitir Cancelamento pelo Usuário"
    *   **Então** o sistema deve aplicar o fluxo de validação financeira (Equipe Financeira) e desativar o cancelamento self-service (US04) para todos os inscritos daquele evento.

## US12: Criação e Edição de Eventos (Ref: RF13)
**Como** organizador
**Quero** criar, editar e excluir as páginas de eventos no sistema
**Para** disponibilizar a programação oficial de forma atualizada no catálogo.

### Critérios de Aceitação (BDD)

*   **Cenário 1: Criação de novo evento**
    *   **Dado** que estou autenticado como organizador
    *   **Quando** eu preencher as informações básicas (título, data, local, limite de vagas e preço) e confirmar a criação
    *   **Então** o evento deve ser publicado e ficar visível no catálogo principal para os participantes.

## US13: Gestão Manual de Participantes (Ref: RF14)
**Como** organizador
**Quero** acessar a lista de participantes inscritos em qualquer evento do sistema
**Para** poder gerenciar as inscrições e intervir manualmente (ex: remover inscrições indevidas).

### Critérios de Aceitação (BDD)

*   **Cenário 1: Remoção de participante por parte da organização**
    *   **Dado** que estou visualizando a lista de inscritos de um evento
    *   **Quando** eu solicitar a remoção de um participante com status "Confirmado"
    *   **Então** a inscrição dele deve ser cancelada internamente e a vaga respectiva deve retornar para o estoque do evento.

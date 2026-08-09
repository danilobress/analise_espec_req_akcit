# Histórias de Usuário - Participante

## US01: Catálogo de Eventos (Ref: RF01)
**Como** participante
**Quero** visualizar um catálogo centralizado com todos os eventos disponíveis
**Para** poder escolher e me inscrever naqueles que são do meu interesse.

### Critérios de Aceitação (BDD)

*   **Cenário 1: Visualização padrão**
    *   **Dado** que acesso a página principal do sistema
    *   **Quando** o catálogo for carregado
    *   **Então** devo visualizar a lista de eventos disponíveis, exibindo título, data e status (aberto, esgotado).

## US02: Inscrição Múltipla em Workshops (Ref: RF02)

**Como** participante
**Quero** me inscrever em múltiplos workshops no mesmo dia
**Para** otimizar meu tempo e aproveitar melhor o evento.

### Critérios de Aceitação (BDD)

*   **Cenário 1: Inscrição em horários distintos**
    *   **Dado** que selecionei dois workshops no mesmo dia com horários diferentes
    *   **Quando** eu confirmar a inscrição
    *   **Então** o sistema deve aprovar e efetivar ambas as inscrições.


## US03: Comprovante Automático (Ref: RF03)
**Como** participante
**Quero** receber um comprovante automático logo após a inscrição
**Para** ter a garantia e o registro da minha participação.

### Critérios de Aceitação (BDD)

*   **Cenário 1: Envio de comprovante após confirmação**
    *   **Dado** que minha inscrição em um evento foi efetivada
    *   **Quando** o sistema processar a confirmação final da vaga
    *   **Então** o participante deve receber ou ter acesso imediato ao seu comprovante.

## US04: Cancelamento Self-Service (Ref: RF04, RN01)
**Como** participante
**Quero** cancelar minha inscrição sem precisar contatar a organização
**Para** gerenciar meus imprevistos com agilidade.

### Critérios de Aceitação (BDD)

*   **Cenário 1: Cancelamento permitido**
    *   **Dado** que estou inscrito em um evento cuja política permite cancelamento
    *   **Quando** eu solicitar o cancelamento através do meu painel
    *   **Então** minha inscrição deve ser cancelada e minha vaga devolvida ao sistema.

*   **Cenário 2: Cancelamento não permitido**
    *   **Dado** que estou inscrito em um evento cuja política não permite cancelamento
    *   **Quando** eu acessar os detalhes da minha inscrição no painel
    *   **Então** o sistema não deve permitir que o cancelamento seja realizado pelo participante.

## US05: Emissão de Certificados (Ref: RF05)
**Como** participante
**Quero** emitir meu certificado após o término do evento
**Para** comprovar minha presença e validar horas complementares.

### Critérios de Aceitação (BDD)

*   **Cenário 1: Certificado liberado**
    *   **Dado** que o evento foi concluído e (se aplicável) minha presença confirmada
    *   **Quando** eu acessar a área de certificados no meu perfil
    *   **Então** devo conseguir gerar e ter acesso ao meu certificado.

*   **Cenário 2: Evento em andamento/não ocorrido**
    *   **Dado** que o evento ainda não ocorreu ou não foi finalizado
    *   **Quando** eu acessar a área de certificados
    *   **Então** o sistema deve informar que o certificado só estará disponível ao fim do evento.

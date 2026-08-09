# Histórias de Usuário - Palestrante

## US11: Consulta à Lista de Participantes (Ref: RF11)
**Como** palestrante
**Quero** acessar e visualizar a lista de participantes inscritos nas atividades onde vou ministrar
**Para** que eu possa conhecer previamente o perfil do meu público e alinhar meu conteúdo.

### Critérios de Aceitação (BDD)

*   **Cenário 1: Acesso autorizado e restrito**
    *   **Dado** que estou autenticado como palestrante da "Oficina A"
    *   **Quando** eu acessar a página de gestão da minha oficina
    *   **Então** devo conseguir visualizar a lista de participantes com inscrição "Confirmada" para aquela atividade.

*   **Cenário 2: Tentativa de acesso não autorizado**
    *   **Dado** que sou palestrante apenas da "Oficina A"
    *   **Quando** tentar acessar os dados da "Oficina B" (onde não leciono)
    *   **Então** o sistema deve exibir uma mensagem de "Acesso Negado" por falta de permissão.

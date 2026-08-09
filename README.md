# Atividade: Análise e Especificação de Requisitos com GenAI


## 🤖 Ferramenta de GenAI Utilizada
Para a execução desta atividade, utilizei o modelo **Google Gemini**.


## 🛠️ Como a IA apoiou as diferentes etapas da atividade
A Inteligência Artificial atuou como uma autêntica parceira cognitiva (*Human-in-the-Loop*) ao longo de todo o processo, apoiando da seguinte forma:

1. **Estruturação de Dados Brutos:** A IA converteu o documento de elicitação em formato de texto simples (.txt) para um formato estruturado (Markdown), destacando declarações de *stakeholders* e criando um ponto de partida organizado.

2. **Análise Crítica e Extração:** Durante o levantamento, a IA varreu os textos para extrair de forma precisa os Requisitos Funcionais e Regras de Negócio, separando o que era sistêmico do que era regra corporativa. O apoio mais valioso foi o seu senso crítico em mapear **lacunas e ambiguidades**, apontando ativamente o que o texto não dizia (prazos, regras de reembolso e concorrência).

3. **Decisão e Especificação:** Na fase final, a IA atuou como arquiteta sugerindo os artefatos de documentação baseando-se no alto volume de regras de exceção do sistema. Em seguida, auxiliou na redação pesada (*pair-writing*), elaborando todo o esqueleto das Histórias de Usuário e gerando os testes lógicos do BDD para estressar os cenários operacionais.



## ✅ Quais sugestões da IA foram aceitas

Foram aceitas sugestão em utilizar Histórias de Usuário atreladas a Critérios de Aceitação BDD. Concordei com a justificativa de que o sistema lida com muitos contextos dinâmicos (inscrição com sucesso, lista de espera, reembolsos negados), com lacunas que ainda estão em aberto e que a estrutura *Dado-Quando-Então* traria a clareza necessária e importante para este projeto. Também acatei a proposta de realizar Wireframes para dar suporte aos key users.


## ❌ Quais sugestões foram descartadas ou modificadas e as justificativas

Foram descartadas ou modificadas alucinações geradas pela IA ao tentar preencher lacunas da elicitação que ainda precisam ser validadas com os key users. As principais alterações foram:

1. Remoção de Critérios de Aceite de Fluxos Não Definidos:

Foram bloqueados/removidos os critérios de aceite (BDD) que tentavam ditar o funcionamento da fila de espera, da política de reembolsos, do ciclo de expiração financeira e de como o conflito de horários seria avisado. Como a elicitação original registrou explicitamente que essas definições estavam pendentes, necessário não assumir esses fluxos, que induziriam a equipe de desenvolvimento ao erro sem o consentimento dos key users.

2. Separação de Requisito de Negócio vs Solução Técnica/UI:

Foram descartadas regras que invadiam o escopo de Design de Interface (UX) ou Arquitetura técnica, como definir que um botão deveria ficar "invisível/desabilitado", que o comprovante iria obrigatoriamente por "e-mail", que o certificado seria em "PDF" ou que o dashboard não deveria "recarregar a página". Histórias de usuário e BDDs devem tratar de comportamentos e regras de negócio, não direcionar solução de forma técnica prematuramente. Para as questões de layout, a solução foi utilizar a construção de Wireframes (Protótipos de Interface de Baixa Fidelidade).

3. Restrições de Privacidade (LGPD):

Foi removida a afirmação do BDD do palestrante de que o sistema "ocultaria dados sensíveis conforme LGPD". A LGPD não foi discutida e definida ainda na elicitação. Ocultar dados pode até ter sido uma boa ideia tecnicamente, mas precisam ter uma definição clara pelos key users antes. Por isso, a decisão de ocultar dados de e-mail e CPF foi incluída estrategicamente como uma proposta dentro da fase de Wireframes, com foco em mostrar para os key users para tomada de decisão visualmente.

4. Adendos ao Glossário:

Foram realizadas alterações nas descrições do Organizador e papéis associados. Algumas atribuições (como parametrizar preços) foram deduzidas pela IA. Necessário descrever no glossário que essas permissões são provisórias até que uma verdadeira Matriz de Acesso seja elaborada com o key users.

5. Alterações Wireframes:

Foram realizadas alterações na apresentação dos Wireframes para ficar mais claro quais pontos dependem de definição dos key users. Foram incluídos novos Wireframes importantes que estavam faltando, como o Dashboard de Gerenciamento e o Catálogo de Eventos, com o objetivo de cobrir os principais cenários e regras de negócio levantadas.


## 🎯 Por que os artefatos escolhidos foram considerados os mais adequados para o projeto

Foram analisadas as elicitações levantadas e foi observado que atualmente existem muitas lacunas e definições que precisam ser realizadas em etapas futuras e para que isso possa ocorrer de uma forma que equilibre agilidade, comunicação mais clara e parte técnica, foram selecionados os artefatos

1. User Stories (Histórias de Usuário): Durante a análise da elicitação, é possível ver que existem lacunas conceituais e indefinições de regras de negócio (tais como políticas de reembolso, prazos de cancelamento e regras de lista de espera) e para que isso possa ocorrer de uma forma não tão engessada como ocorre em casos de uso tradicionais, foi escolhido o modelo de User Story, para poder ter um fluxo mais ágil de definição e dar suporte ao que os usuários precisam diretamente.

2. BDD (Behavior-Driven Development): Para atuar em conjunto com a User Story e ter uma visão melhor do que é esperado foram utilizados critérios de aceitação em BDD (Dado-Quando-Então), onde os critérios vão orientar todo o time no que devemos esperar dos cenários, dando suporte para os desenvolvedores implementarem, os testadores criarem os casos de teste e até mesmo o key users analisarem se estamos no caminho correto, analisando esses critérios de aceite.

3. Protótipos de Interface (Wireframes de Baixa Fidelidade): Foram criados Protótipos de Interface (Wireframes) para fornecer uma visão inicial das telas principais, sanando dúvidas de usabilidade e fluxos de navegação e com isso trazer questões importantes sem definição ainda em formato de proposta e permitir que os key users forneçam feedbacks rápidos e identifiquem problemas de navegação de forma inicial, reduzindo drasticamente o risco de retrabalho na fase de desenvolvimento.

4. Glossário do Projeto: Diante da diversidade de perfis de stakeholders (palestrantes, equipe financeira, organizadores e TI) foi criado um glossário para unificar o vocabulário. Ele busca ajudar a eliminar ambiguidades causadas por terminologias que acabam conflitando levantadas nas entrevistas e auxilia em um entendimento comum sobre o domínio do negócio para todos os envolvidos.

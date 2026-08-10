# Matriz de Rastreabilidade

Este documento apresenta a Matriz de Rastreabilidade, garantindo que todos os Requisitos Funcionais (RF), Regras de Negócio (RN) e Requisitos Não Funcionais (RNF) elicitados estejam devidamente mapeados.

> [!NOTE]
> **Fase Atual (Discovery & Especificação):** Colunas técnicas e colunas de teste foram omitidas nesta versão, pois não há código construído para mapear e os testes ainda serão gerados futuramente.
> **Aviso sobre Prioridade:** A coluna de prioridade utiliza o framework MoSCoW. A classificação atual reflete uma proposta técnica preliminar baseada na análise de requisitos (onde Alta = Must Have, Média = Should Have / Could Have) e carece de validação final junto à área de Negócio / PO.

| Origem (Req/Regra) | Prioridade | História de Usuário / Mapeamento | Ator (Perfil) | Artefato de Apoio (UX) | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| [RF01](../analise/requisitos-funcionais.md) - Catálogo de eventos | Must Have | [US01: Catálogo de Eventos](historias-participante.md) | Participante | [Tela 3: Catálogo de Eventos](wireframes.md) | Especificado |
| [RF02](../analise/requisitos-funcionais.md) - Inscrição múltipla | Should Have | [US02: Inscrição Múltipla em Workshops](historias-participante.md) | Participante | [Tela 1: Conflito de Horários](wireframes.md) | Especificado |
| [RF03](../analise/requisitos-funcionais.md) - Emissão de comprovante | Should Have | [US03: Comprovante Automático](historias-participante.md) | Participante | - | Especificado |
| [RF04](../analise/requisitos-funcionais.md), [RN01](../analise/regras-de-negocio.md) - Cancelamento | Must Have | [US04: Cancelamento Self-Service](historias-participante.md) | Participante | [Tela 2: Regra de Cancelamento](wireframes.md) | Especificado |
| [RF05](../analise/requisitos-funcionais.md) - Certificados | Must Have | [US05: Emissão de Certificados](historias-participante.md) | Participante | - | Especificado |
| [RF06](../analise/requisitos-funcionais.md) - Controle de vagas | Must Have | [US06: Controle Automático de Vagas](historias-organizador.md) | Organizador | [Tela 3: Catálogo de Eventos](wireframes.md) | Especificado |
| [RF07](../analise/requisitos-funcionais.md) - Fila de espera | Should Have | [US07: Lista de Espera Automática](historias-organizador.md) | Organizador / Participante | [Tela 3: Catálogo de Eventos](wireframes.md) | Especificado |
| [RF08](../analise/requisitos-funcionais.md) - Dashboard | Could Have | [US08: Dashboard em Tempo Real](historias-organizador.md) | Organizador | [Tela 5: Dashboard do Organizador](wireframes.md) | Especificado |
| [RF09](../analise/requisitos-funcionais.md), [RF12](../analise/requisitos-funcionais.md) - Regras | Must Have | [US09: Configuração de Regras](historias-organizador.md) | Organizador | - | Especificado |
| [RF10](../analise/requisitos-funcionais.md), [RN03](../analise/regras-de-negocio.md) - Financeiro | Must Have | [US10: Validação de Pagamentos](historias-financeiro.md) | Equipe Fin. | - | Especificado |
| [RF11](../analise/requisitos-funcionais.md) - Consulta participantes | Should Have | [US11: Consulta à Lista](historias-palestrante.md) | Palestrante | [Tela 4: Painel do Palestrante](wireframes.md) | Especificado |
| [RF13](../analise/requisitos-funcionais.md) - Gestão de eventos | Must Have | [US12: Criação e Edição de Eventos](historias-organizador.md) | Organizador | - | Especificado |
| [RF14](../analise/requisitos-funcionais.md) - Gestão manual | Should Have | [US13: Gestão Manual de Participantes](historias-organizador.md) | Organizador | - | Especificado |
| [RN02](../analise/regras-de-negocio.md) - Direito a Reembolso | Must Have | *Depende de Definição com Negócio* | - | [Lacunas](../analise/duvidas-e-lacunas.md) | Pendente |
| [RN04](../analise/regras-de-negocio.md) - Simultaneidade | Should Have | *Regra validada junto à [US02](historias-participante.md)* | Participante | [Tela 1: Conflito de Horários](wireframes.md) | Especificado |
| [RNF01](../analise/requisitos-nao-funcionais.md) - Concorrência (Vagas) | Must Have | *Restrição Arquitetural / Back-end* | Sistema | - | Pendente |
| [RNF02](../analise/requisitos-nao-funcionais.md) - Envio Automatizado | Should Have | *Restrição Arquitetural / Integração* | Sistema | - | Pendente |
| [RNF03](../analise/requisitos-nao-funcionais.md) - Usabilidade Simples | Must Have | *Diretriz de UX/UI* | Participante | [Wireframes](wireframes.md) | Especificado |
| [RNF04](../analise/requisitos-nao-funcionais.md) - Segurança e LGPD | Must Have | *Restrição Arquitetural* | Sistema | [Tela 4: Painel do Palestrante](wireframes.md) | Pendente |
| [RNF05](../analise/requisitos-nao-funcionais.md) - Disponibilidade (SLA) | Must Have | *Restrição Arquitetural / Infraestrutura* | Sistema | - | Pendente |
| [RNF06](../analise/requisitos-nao-funcionais.md) - Acessibilidade | Should Have | *Diretriz de Front-end (WCAG)* | Participante | - | Pendente |
| Lacunas Macro (Login, SSO, Pagamentos) | Must Have | *Requisitos a Descobrir* | Vários | [Lacunas](../analise/duvidas-e-lacunas.md) | Pendente |

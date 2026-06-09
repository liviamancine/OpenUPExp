
# Fase de Elaboração (OpenUP4Exp)

Segunda fase do processo.
A fase de Elaboração tem como objetivo estabelecer três artefatos principais Elicitação de Explicabilidade[Explainability Needs](../artefatos/explainability-needs.md), Análise de Explicabilidade [Refined Explainability Requirements](../artefatos/refined-explainability-requirements.md) e Especificação da Explicabilidade [User Stories](user-stories.md), que compõem o [Documento de Requisitos de Explicabilidade (DRE)](DRE.md).

Descrição Principal

O propósito desta fase no OpenUPExp é atenuar os riscos técnicos e não técnicos relacionados à incorporação da explicabilidade em sistemas baseados em Inteligência Artificial. Durante essa fase, busca-se estabelecer uma base sólida para a operacionalização da explicabilidade, refinando os requisitos previamente identificados e definindo mecanismos arquiteturais e organizacionais capazes de sustentar explicações compreensíveis, rastreáveis e adequadas aos diferentes stakeholders.

Os riscos técnicos são tratados por meio da definição e validação inicial da arquitetura explicável do sistema, incluindo mecanismos de geração, apresentação, rastreabilidade e gerenciamento das explicações. Já os riscos não técnicos são tratados em estreita colaboração com os stakeholders, permitindo responder questões como:

- Os stakeholders compreendem e concordam com as explicações fornecidas pelo sistema?
- Os mecanismos de explicabilidade propostos atendem às necessidades de transparência e compreensão?
- As explicações produzidas são adequadas aos diferentes perfis de usuários?
- Existem restrições regulatórias, éticas ou organizacionais que impactam a explicabilidade?
- A equipe possui conhecimento técnico suficiente para implementar mecanismos de explicabilidade?
- Os componentes, modelos ou bibliotecas utilizados suportam os níveis de explicabilidade esperados?
- A arquitetura proposta permite rastreabilidade e auditoria das decisões automatizadas?

## Objetivos da fase de elaboração 

Obter um entendimento mais detalhado dos requisitos de explicabilidade

Refinar e detalhar os requisitos de explicabilidade identificados na fase de Concepção, consolidando:

- os pontos de decisão que requerem explicação;
- os stakeholders que necessitam de explicações;
- os tipos de explicação esperados;
- os critérios de qualidade das explicações;
- os limites e restrições da explicabilidade.

Esse refinamento permite maior alinhamento entre stakeholders, equipe técnica e arquitetura do sistema.

---

## Atenuar riscos relacionados à explicabilidade

Identificar e reduzir riscos associados à implementação da explicabilidade, incluindo:

- limitações técnicas dos modelos de IA
- impacto da explicabilidade no desempenho do sistema
- dificuldades de compreensão das explicações
- restrições legais e regulatórias
- riscos de exposição indevida de informações sensíveis
- dependência de componentes externos ou bibliotecas de explicabilidade

O detalhamento dos requisitos e a validação inicial da arquitetura permitem produzir estimativas mais precisas de custo, esforço e cronograma.

---

## Principais Considerações

A quantidade de iterações na fase de Elaboração do OpenUPExp depende de fatores como:

- criticidade do sistema
- complexidade dos requisitos de explicabilidade
- maturidade da arquitetura de IA
- nível de risco associado às decisões automatizadas
- necessidade de conformidade regulatória
- diversidade de stakeholders envolvidos

Projetos com baixa complexidade ou manutenção incremental podem combinar atividades de Concepção e Elaboração em poucas iterações. Já sistemas inéditos ou de alto risco podem demandar múltiplas iterações para validar:

- mecanismos de explicabilidade
- qualidade das explicações
- aderência regulatória
- cobertura arquitetural dos cenários explicáveis

Nessas situações, recomenda-se iniciar pela implementação e validação de cenários críticos de explicabilidade, refinando progressivamente os mecanismos arquiteturais e os requisitos ao longo das iterações. 

---

## Informações Adicionais

| **Conceito** | VERIFICAR O QUE É NECESSÁRIO|
|--------------|----------------------|
|              | • [Ciclo de Vida do Projeto](#) <br> • [Colaborar para Alinhar Interesses](#) <br> •[Equilibrar Prioridades Concorrentes](#) <br> • [Iteração](#) |
                  
---
Observação sobre o framework
Conforme o processo evolui, o [DRE](DRE.md) é continuamente atualizado a cada iteração e interação das fases seguintes (Concepção e Elaboração), incorporando novos requisitos, refinamentos arquiteturais, decisões de projeto e resultados de testes de usabilidade (VALIDAR) e validação de explicabilidade.

Esse processo incremental assegura que a explicabilidade seja tratada como um requisito não funcional essencial, integrado desde a concepção e evoluindo conforme o conhecimento sobre o sistema também evolui.

---
>  **Dica:** Este documento é parte do *OpenUP4Exp* — uma instanciação do OpenUP voltada à Engenharia de Requisitos para sistemas baseados em Inteligência Artificial com foco na Explicabilidade.

---

##Referência
{file:///C:/Users/Livia%20Mancine/Downloads/OpenUP/Publish/openup/guidances/concepts/project_lifecycle_203F87.html}
{file:///C:/Users/Livia%20Mancine/Downloads/OpenUP/Publish/openup/guidances/concepts/elaboration_phase_BE880435.html}

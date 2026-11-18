# Tarefa: Analisar Requisitos de Explicabilidade (Passos)

**Descrição:**  
Definir a análise dos requisitos de explicabilidade

Observação:

- O problema de explicabilidade já foi reconhecido durante a fase de Concepção.
- A Visão da Explicabilidade foi definida e fornece o contexto estratégico para a análise.
- Os requisitos de explicabilidade foram elicitados e representam as necessidades iniciais dos stakeholders, embora ainda possam ser refinados ao longo do projeto.
- Nesta tarefa, os requisitos são analisados quanto à sua consistência, aos aspectos de qualidade que ajudam a alcançar, à viabilidade, às dependências, aos conflitos e às prioridades, sendo posteriormente refinados e associados aos aspectos explicativos mais adequados.
- A explicabilidade é tratada como um requisito-meio: cada requisito de explicabilidade deve estar associado a pelo menos um aspecto de qualidade (fim) que justifique sua existência. Essa associação é apoiada pela Taxonomia meio-fim de explicabilidade.
- O resultado desta atividade constitui a base para a especificação detalhada dos requisitos de explicabilidade na tarefa **Especificar os Requisitos de Explicabilidade**.

[Disciplina: Requisitos](requisitos.md)

**Objetivo**

A análise de explicabilidade tem como objetivo transformar as necessidades de explicação em mecanismos explicativos adequados, explicitando para quais aspectos de qualidade do sistema de IA cada requisito de explicabilidade contribui.

## Relacionamentos

**Papéis**  
- **Executor Principal:** [Engenheiro de Requisitos](../papeis/engenheiro-requisitos.md)  
- **Executores Adicionais:** [Arquiteto de Software](../papeis/arquiteto-software.md), [Gerente de Projetos](../papeis/gerente-projeto.md), 
[Especialista Ética](../papeis/especialista-etica-regulacao) e [Stakeholders](../papeis/stakeholders)

**Entradas**  
- **Obrigatório:**  
  - Escopo do Projeto
  - Necessidade da Explicabilidade Reconhecida
  - Elicitação dos requisitos de explicabilidade
  - Taxonomia meio-fim de explicabilidade (Catálogo de aspectos de qualidade, Catálogo de requisitos de explicabilidade e Matriz de contribuições)

- **Opcional:**  
  - [Lista de Item de Trabalho](#)
  - Base de normas e leis (apoio à verificação de Compliance e Fairness)

- **Saídas Intermediárias:**  
  - [Glossário](#)
  - [Lista de Item de Trabalhos](#)
  - Mapa de contribuições meio-fim
  - [Documento de Requisitos de Explicabilidade - DRE](../artefatos/DRE.md)
---

## Passos
***1. Consolidar e Caracterizar requisitos de explicabilidade***

**O que fazer**

Analisar cada requisito de explicabilidade identificado durante a elicitação para compreender seu contexto de uso e seus objetivos. O propósito desta atividade é obter informações suficientes para apoiar a seleção de aspectos explicativos adequados, a associação a aspectos de qualidade e a identificação de possíveis riscos, conflitos ou limitações.

Para cada requisito, validar:

- Em qual contexto a explicação será utilizada
- Qual o impacto da decisão apoiada pelo sistema
- Quais requisitos regulatórios, éticos ou organizacionais estão associados

**Quem**

- Engenheiro de Requisitos (líder), com apoio dos Stakeholders, Especialistas de Domínio e Especialistas em IA.

**Onde registrar**

- [Documento de Requisitos de Explicabilidade - DRE](../artefatos/DRE.md) 

**Boas Práticas**

- Considerar diferentes perfis de stakeholders
- Registrar o contexto de uso da explicação
- Avaliar o impacto da decisão apoiada pelo sistema
- Identificar requisitos regulatórios associados
- Usar, sempre que possível, os mesmos termos do Catálogo de requisitos de explicabilidade para os elementos de informação (por exemplo, "limitações", e não "restrições" em um requisito e "limitações" em outro).

  *Perguntas úteis*
- Quem utilizará a explicação?
- Qual decisão está sendo apoiada?
- Qual o risco associado à decisão?
- Qual o objetivo principal da explicação?
- Existe obrigação regulatória para explicar a decisão?
- Existe obrigação regulatória para explicar a decisão?


***2. Classificar aspectos explicativos***

**O que fazer**

Classificar os requisitos de acordo com o aspecto explicativo predominante. Essa classificação auxilia na escolha dos aspectos explicativos mais adequados e facilita a análise posterior.

O aspecto explicativo descreve a natureza da explicação (o que o stakeholder quer fazer com ela). Ele não se confunde com o aspecto de qualidade do passo 3, que descreve a qualidade do sistema de IA que a explicação ajuda a alcançar.

Exemplo:

| Aspectos      | Exemplos                |
| ------------- | ----------------------- |
| Compreensão   | entender resultado      |
| Justificativa | justificar decisão      |
| Confiança     | aumentar aceitação      |
| Auditoria     | verificar comportamento |
| Contestação   | questionar decisão      |
| Aprendizado   | ensinar funcionamento   |


**Quem**

- Engenheiro de Requisitos (facilitador) e Stakeholders.

**Onde registrar**

- [Documento de Requisitos de Explicabilidade - DRE](../artefatos/DRE.md) 

**Boas Práticas**

-  Permitir múltiplas classificações para um mesmo requisito quando necessário.
-  Validar a classificação junto aos stakeholders.
-  Evitar assumir que todos os usuários possuem os mesmos objetivos.

 ***3. Mapear para tipos de explicação***

**O que fazer**

Associar cada requisito de explicabilidade (meio) aos aspectos de qualidade do sistema de IA (fins) para os quais ele contribui, utilizando a Taxonomia meio-fim de explicabilidade.

- Contribuição principal: identificar no Catálogo de requisitos de explicabilidade o requisito correspondente e o aspecto de qualidade para o qual ele foi formulado. Registrar a intensidade da contribuição:
    Make (++): disponibilizar a informação é o próprio aspecto (por exemplo, Transparency).
    Help (+): a explicação contribui, mas o aspecto depende também da pessoa ou de outros elementos do sistema.
    Some+: a contribuição é positiva, mas de grau incerto.

- Contribuições secundárias: quando o requisito compartilha um elemento de informação ou uma característica da explicação com outro requisito do catálogo, ele também  contribui para o aspecto de qualidade desse outro requisito. Essas contribuições são registradas como Some+.
- Revisão pelo engenheiro: aceitar, ajustar ou promover cada contribuição (por exemplo, de Some+ para Help), conforme o contexto do projeto.
- Requisitos não cobertos: quando o requisito não se associa a nenhum aspecto da taxonomia, o engenheiro de requisitos decide como proceder, por exemplo, encaminhá-lo à análise de conflitos (passo 5) ou questionar sua necessidade junto aos stakeholders. A decisão e sua justificativa devem ser registradas.
- Verificação de cobertura (opcional): identificar os aspectos de qualidade que não foram alcançados por nenhum requisito e avaliar, com os stakeholders, se algum deles é relevante para o projeto. Em caso afirmativo, o Catálogo de requisitos de explicabilidade sugere o requisito correspondente.

Aspectos de qualidade da taxonomia:

| Aspecto de qualidade                     | Requisito-meio principal (resumo)         |
| ---------------------------------------- | -------------------------- |
| Trustworthiness                          | Fundamentos dos resultados, evidências e limitações         |
| Transparency                             | Funcionamento, dados, fatores considerados e limitações          |
| Understandability                        | Explicações compreensíveis e adequadas ao perfil e ao contexto         |
| Usability                                | Explicações acessíveis e integradas às tarefas  |
| User Experience                          | Explicações contextualizadas e adequadas às necessidades     |
| User Satisfaction                        | Explicações que atendem às necessidades de informação e às expectativas |
| User Awareness                           | Contexto de uso, comportamento e limitações |
| AI Acceptance                            | Utilidade, funcionamento e adequação dos resultados|
| Ethics                                   | Fundamentos e consequências das decisões|
| Stakeholder Trust                        | Evidências, incertezas e limitações|
| Compliance                               | Evidências sobre desenvolvimento, operação e resultados|
| Fairness                                 | Fatores considerados na produção dos resultados|

**Quem**

Engenheiro de Requisitos (líder), Stakeholders e Especialista em Ética e Regulação (para Ethics, Compliance e Fairness).

**Onde registrar**

- Mapa de contribuições meio-fim (requisito, aspecto de qualidade, tipo de contribuição, rótulo e justificativa)
- [Documento de Requisitos de Explicabilidade - DRE](../artefatos/DRE.md) 


**Boas práticas**
- O fim é sempre uma qualidade do sistema de IA, nunca a própria explicação. As características desejáveis da explicação ficam no texto do requisito.
- Justificar cada contribuição no formato: [o que a explicação disponibiliza] + permite/favorece + [quem] + [efeito no aspecto].
- Em Stakeholder Trust, o objetivo não é aumentar a confiança indiscriminadamente, e sim permitir que os stakeholders calibrem sua confiança.
- Em Compliance e Fairness, consultar a base de normas e leis aplicáveis.
- Registrar os requisitos não cobertos pela taxonomia; eles apoiam a evolução da taxonomia.

---
***4. Analisar conflitos e divergências***

**O que fazer**

Associar cada requisito de explicabilidade a um ou mais tipos de explicação que melhor atendam ao perfil do stakeholder, ao contexto da decisão, ao objetivo da explicação e ao aspecto de qualidade associado no passo 3. O aspecto de qualidade orienta o conteúdo da explicação: por exemplo, calibrar a confiança exige apresentar incertezas e limitações; Compliance exige evidências verificáveis. O objetivo não é selecionar uma ferramenta específica, mas identificar quais abordagens explicativas possuem maior aderência às necessidades identificadas.

Exemplo:

|Necessidade    |Tipo de Explicação                         |
----------------|-------------------------------------------|
|Justificativa clínica          |	Feature Importance        |
|Explicar caso específico	      |Local Explanation          |
|Explicar comportamento geral	  |Global Explanation         |
|Demonstrar exemplos semelhantes|	Example-based Explanation |
|Mostrar regras                 |	Rule-based Explanation    |
|Mostrar impacto dos atributos  |	Counterfactual Explanation|


**Quem**

Engenheiro de Requisitos, Stakeholders, Especialistas de Domínio e Especialistas em IA

**Onde registrar**

- [DRE] - ver onde registrar

**Boas Práticas**

- Priorizar mecanismos compatíveis com o perfil do usuário.
- Considerar limitações dos modelos de IA utilizados.
- Considerar o aspecto de qualidade associado ao requisito na escolha do tipo de explicação.
- Registrar justificativas para o mapeamento realizado.

---
***5. Analisar conflitos e divergências***

**O que fazer**

Identificar conflitos entre requisitos, stakeholders e objetivos de explicabilidade.

Exemplos:

- Usuários desejam explicações simples enquanto auditores exigem alto detalhamento.
- Requisitos de transparência entram em conflito com requisitos de privacidade.
- Explicações mais detalhadas impactam requisitos de desempenho.

Documentar os conflitos identificados e propor alternativas de resolução.

Observação: a taxonomia meio-fim registra apenas contribuições positivas. Contribuições negativas da explicabilidade (por exemplo, sobre security, privacy ou desempenho) e requisitos encaminhados no passo 3 são tratados neste passo.

**Quem**

Engenheiro de Requisitos, Stakeholders, Especialistas de Domínio e Especialistas em IA

**Onde registrar**

[DRE] - ver onde registrar

Boas Práticas

- Registrar explicitamente os conflitos identificados.
- Envolver stakeholders afetados na resolução.
- Documentar justificativas para as decisões tomadas.


***6. Analisar dependências e restrições***

**O que fazer**

Identificar as dependências entre requisitos e as restrições (técnicas, regulatórias e organizacionais) que os afetam, e avaliar o impacto dessas restrições nos requisitos.

As contribuições secundárias do Mapa de contribuições meio-fim indicam requisitos complementares: requisitos que compartilham elementos de informação (por exemplo, evidências ou limitações) e, por isso, contribuem para os mesmos aspectos de qualidade.

Exemplo:

Requisito RE-01 - Depende de rastreabilidade - Impactado pela LGPD

**Quem**

Engenheiro de Requisitos (facilitador), Stakeholders, Gerente de Projeto, Arquiteto.

**Onde registrar**

- [DRE]

**Boas Práticas**

- [VAMOS TER UM DOCUMENTO INDICANDO BOAS PRÁTICAS?](#)

***8. Avaliar viabilidade dos requisitos***

**O que fazer**

Avaliar se cada requisito de explicabilidade pode ser atendido considerando as características do sistema de IA, as restrições do projeto e o contexto de utilização. A avaliação deve verificar se o requisito é tecnicamente implementável, operacionalmente aplicável e compatível com aspectos regulatórios, organizacionais e de negócio. Deve-se considerar os riscos, limitações e premissas para apoiar a priorização e a especificação dos requisitos nas etapas seguintes.
Sugestão: matriz de avaliação de viabilidade:

| Critério                        | Observação                                    | Situação|
| ------------------------------- | ----------------------------------------------|---------|
| Viabilidade técnica             | O modelo suporta explicações locasis          |Sim/Não  |
| Viabilidade regulatória         | Atende às exigências da LGPD                  |Sim/Não  |
| Viabilidade operacional         | Compatível com o fluxo de trabalho do usuário |Sim/Não  |
| Viabilidade econômica           | Custo aceitável para o projeto                |Sim/Não  |



**Quem**

Engenheiro de Requisitos (facilitador), Arquiteto de Software, Especialista em IA, Especialista de domínio,  Gerente de Projeto e Stakeholders (quando necessário).

**Onde registrar**

- [DRE] 

**Boas Práticas**

- Avaliar a viabilidade antes da especificação detalhada dos requisitos.
- Considerar simultaneamente aspectos técnicos, regulatórios e organizacionais.
- Registrar premissas e restrições que possam impactar a implementação.
- Identificar riscos que possam comprometer a qualidade ou a efetividade das explicações.
- Revisar a viabilidade sempre que houver mudanças significativas nos requisitos, na arquitetura ou no modelo de IA.

***7. Priorizar requisitos usando MoScoW***

**O que fazer**

Priorizar os requisitos de explicabilidade analisados utilizando a técnica MoSCoW, classificando-os de acordo com sua importância para o atendimento das necessidades dos stakeholders, dos objetivos do sistema e das restrições do projeto.

Cada requisito deve ser classificado em uma das seguintes categorias:

- Must Have: requisito essencial para que o sistema atenda aos objetivos mínimos de explicabilidade.
- Should Have: requisito importante, mas cuja ausência não inviabiliza o sistema.
- Could Have: requisito desejável, cuja implementação agrega valor, mas pode ser adiada.
- Won't Have (for now): requisito reconhecido, porém fora do escopo da iteração ou da versão atual.

  O Mapa de contribuições meio-fim apoia a priorização: requisitos que contribuem para mais aspectos de qualidade tendem a ser mais importantes, e requisitos sem aspecto de qualidade associado devem ter sua necessidade questionada.

**Quem**

Engenheiro de Requisitos (facilitador), Stakeholders, Gerente de Projeto, Arquiteto de Software

**Onde registrar**

- [DRE]

**Boas Práticas**

- Priorizar requisitos após a análise de conflitos, dependências e viabilidade.
- Justificar a classificação atribuída a cada requisito.
- Revisar a priorização sempre que novos requisitos forem identificados ou houver mudanças significativas no projeto.
- Buscar equilíbrio entre necessidades dos stakeholders, riscos e capacidade de implementação.

***9. Obter consenso***

**O que fazer**

Conduzir uma revisão colaborativa dos requisitos de explicabilidade refinados com os stakeholders e a equipe do projeto, buscando validar os resultados da análise realizada e estabelecer um entendimento comum sobre os requisitos que seguirão para a etapa de especificação.

**Quem**

Engenheiro de Requisitos (facilitador), Stakeholders, Gerente de Projeto, Arquiteto de Software, Especialista em IA, Especialista de domínio (quando aplicável).

**Onde registrar**

- [DRE] 

**Boas Práticas**

- Promover revisões colaborativas envolvendo representantes dos principais stakeholders.
- Registrar justificativas para decisões, conflitos resolvidos e requisitos adiados.
- Garantir que todos os requisitos priorizados possuam consenso suficiente antes da especificação.
- Verificar a rastreabilidade entre os requisitos elicitados, os requisitos refinados e a Visão da Explicabilidade.


---

## Informações Adicionais

**Listas de Verificação:**  
- [Documento de Visão de Explicabilidade](../tarefas/documento-requisito.md) 

**Conceitos:**  
- [Requisitos](#)
- Taxonomia meio-fim de explicabilidade Diretrizes:
- Revisão eficaz de Requisitos
- Técnicas Para Obtenção de Requisitos de Explicabilidade

 
---
**Referências:**  
- [Link para o OpenUP Original](file:///C:/Users/Livia%20Mancine/Downloads/OpenUP/Publish/openup/tasks/define_vision_9D36CF2F.html)



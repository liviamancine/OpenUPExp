# Tarefa: Encontrar e Descrever Requisitos de Explicabilidade (Passos)

**Descrição:** 

Esta tarefa descreve como identificar os requisitos de explicabilidade de sistemas baseados em Inteligência Artificial, de forma que o escopo das necessidades de explicação possa ser determinado e alinhado aos objetivos dos stakeholders.

Observação:
Os resultados obtidos servem como base para a definição da Visão da Explicabilidade e para o posterior detalhamento dos requisitos de explicabilidade.

[Disciplina: Requisitos](../disciplina/requisitos.md)

**Objetivo**

O propósito desta tarefa é identificar os requisitos de explicabilidade associados ao sistema baseado em Inteligência Artificial. Esses requisitos estabelecem uma compreensão compartilhada entre stakeholders e equipe de desenvolvimento sobre as necessidades de explicação e compreensão das decisões apoiadas pelo sistema. Os requisitos identificados constituem a base para a definição da Visão da Explicabilidade e para o alinhamento das expectativas dos stakeholders quanto ao que deve ser explicado, para quem as explicações serão fornecidas e em quais contextos elas serão utilizadas.

O objetivo é obter uma compreensão inicial das necessidades de explicabilidade em um nível estratégico, permitindo delimitar o escopo da explicabilidade, identificar stakeholders relevantes, reconhecer restrições e expectativas associadas às explicações e estabelecer uma base para o posterior detalhamento dos requisitos de explicabilidade. Informações mais específicas sobre conteúdo, formato, mecanismos e níveis de explicação serão refinadas em atividades posteriores da Engenharia de Requisitos.

## Relacionamentos

**Papéis**  
- **Executor Principal:** [Engenheiro de Requisitos](../papeis/engenheiro-requisitos.md)  
- **Executores Adicionais:** [Arquiteto de Software](../papeis/arquiteto-software.md), [Desenvolvedor](../papeis/desenvolvedor.md), [Especialista de Domínio](../papeis/especialista-dominio.md), [Stakeholders](../papeis/stakeholders.md)[Testador](../papeis/testador.md), [Especialista Regulação](../papeis/especialista-etica-regulacao.md), [Especialista em IA](../papeis/especialista-IA.md)

**Entradas**  
- **Obrigatório:**  
  - [Glossário](../artefatos/glossario.md) 
  - [Visão da Explicabilidade](../artefatos/visao-explicabilidade.md)
- **Opcional:**  
  - Nenhum
- **Saídas:**  
  - [Glossário](../artefatos/glossario.md)
  - [Especificação da Explicabilidade](../artefatos/DRE.md)
---
## Passos

***1. Obter Informações ***
**O que fazer**
Identificar e coletar informações relevantes sobre o sistema baseado em Inteligência Artificial, seu contexto de uso, os stakeholders envolvidos, os processos decisórios apoiados e as necessidades iniciais de explicabilidade. A elicitação pode ser realizada por meio de entrevistas, workshops, observação de atividades, análise documental, protótipos ou outras técnicas adequadas ao contexto do projeto.

O objetivo é compreender:

- quais decisões são apoiadas pelo sistema;
- quais stakeholders são impactados;
- quais preocupações existem em relação à transparência e compreensão das decisões;
- quais restrições regulatórias, organizacionais ou éticas devem ser consideradas.

**Quem**

Engenheiro de Requisitos, Stakeholders, Especialistas de Domínio e Especialistas em IA (quando aplicável)

**Onde registrar**
[Visão da Explicabilidade](../artefatos/visao-explicabilidade.md)
[Glossário](../artefatos/glossario.md)

**Boas Práticas**
- Identificar stakeholders com diferentes perspectivas e responsabilidades.
- Investigar situações em que explicações serão necessárias para apoiar decisões.
- Considerar requisitos legais, regulatórios e organizacionais relacionados ao uso de IA.
- Evitar discutir soluções de explicabilidade neste momento; o foco deve permanecer na compreensão das necessidades.
- Registrar dúvidas, conflitos e riscos identificados durante a elicitação.

*Veja Guideline*

Técnicas para obtenção de requisitos de explicabilidade??? - para mais informações

***2. Identifique e capture os termos do domínio***

**O que fazer**
Identificar, documentar e manter um vocabulário comum entre os stakeholders e a equipe de desenvolvimento. Os termos devem representar conceitos relevantes do domínio da aplicação, do sistema de Inteligência Artificial e das necessidades de explicabilidade. A atividade busca reduzir ambiguidades e promover um entendimento compartilhado dos conceitos utilizados durante a elicitação e especificação dos requisitos.

Além dos termos do domínio do negócio, recomenda-se identificar conceitos relacionados à explicabilidade, transparência, rastreabilidade, interpretação, explicação, recomendação, confiança, viés e outros conceitos relevantes para o contexto do sistema.

**Quem**

Engenheiro de Requisitos
Stakeholders
Especialistas de Domínio
Especialistas em IA/AM (quando aplicável)

**Onde registrar**

[Glossário](../artefatos/glossario.md)


**Boas Práticas**

- Definir termos utilizando linguagem clara e objetiva.
- Registrar sinônimos, siglas e acrônimos relevantes.
- Evitar definições excessivamente técnicas quando o termo for utilizado por stakeholders não especialistas.
- Validar os significados junto aos especialistas do domínio.
- Atualizar o glossário continuamente à medida que novos termos forem identificados.
- Garantir consistência entre os termos utilizados nos artefatos do projeto.


***3. Identificar os tipos de requisitos de explicabilidade relevantes ao sistema***

**O que fazer**
Identificar quais necessidades de explicabilidade são relevantes para o sistema e para seus stakeholders. O objetivo é compreender quais aspectos das decisões, recomendações ou previsões produzidas pelo sistema precisam ser explicados. Os requisitos identificados podem estar relacionados à compreensão, justificativa, transparência, rastreabilidade, auditoria, conformidade regulatória, confiança ou outros objetivos associados à explicabilidade.

Esta atividade auxilia na definição do escopo inicial da explicabilidade e na identificação dos aspectos que deverão ser posteriormente detalhados.
**Quem**

Engenheiro de Requisitos, Especialistas de Domínio e Especialistas em IA (quando aplicável)

**Onde registrar**

[[Visão da Explicabilidade](../artefatos/visao-explicabilidade.md)
[Glossário](../artefatos/glossario.md)

**Boas Práticas**

- Focar inicialmente nos objetivos da explicabilidade, e não nas técnicas de explicação.
- Identificar diferentes necessidades para diferentes perfis de stakeholders.
- Considerar requisitos regulatórios, éticos e organizacionais relacionados à transparência.
- Avaliar quais decisões possuem maior impacto e demandam maior nível de explicação.
- Registrar conflitos ou divergências entre expectativas dos stakeholders.

***4. Identificar os stakeholders e suas necessidades de explicabilidade***

**O que fazer**
Identificar os stakeholders que interagem, utilizam, supervisionam ou são impactados pelas decisões apoiadas pelo sistema baseado em Inteligência Artificial.
Para cada stakeholder, identificar quais informações precisam ser explicadas, os objetivos dessas explicações, o contexto de uso e as expectativas relacionadas à compreensão das decisões do sistema.
Esta atividade auxilia na definição do escopo inicial da explicabilidade e na identificação dos aspectos que deverão ser posteriormente detalhados.

**Quem**

Engenheiro de Requisitos, Especialistas de Domínio e Stakeholders.

**Onde registrar**

[[Visão da Explicabilidade](../artefatos/visao-explicabilidade.md)

**Boas Práticas**

- Considerar usuários finais, operadores, gestores, reguladores e demais partes interessadas.
- Identificar diferentes níveis de conhecimento técnico entre os stakeholders.
- Registrar objetivos distintos para as explicações, como compreensão, confiança, auditoria ou conformidade.
- Evitar assumir que todos os stakeholders possuem as mesmas necessidades de explicabilidade.
- Validar as necessidades identificadas diretamente com os stakeholders.






## Informações Adicionais

**Listas de Verificação:**  
- [Documento de Visão de Explicabilidade](../tarefas/documento-requisito.md) 

**Conceitos:**  
- [Requisitos](#)

  **Diretrizes:**  
- [Revisão eficaz de Requisitos](#)
- [Técnicas Para Obtenção de Requisitos de Explicabilidade](#)
---
**Referências:**  
- [Link para o OpenUP Original]

🧩 **OpenUP4ER — Framework de Engenharia de Requisitos para Explicabilidade em Sistemas de IA**


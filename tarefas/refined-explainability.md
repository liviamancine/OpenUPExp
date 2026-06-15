# Tarefa: Refined Explainability Requirements (Passos)

**Descrição:**  
Definir a análise dos requisitos de explicabilidade

Observação:
- o problema de explicabilidade já foi reconhecido fora do OpenUPExp (escopo do projeto)
- o OpenUPExp começa quando há a necessidade explícita de explicabilidade
- os requisitos de explicabilidade foram elicitados, não em sua totalidade, mas alg

[Disciplina: Requisitos](requisitos.md)

**Objetivo**

A análise de explicabilidade tem como objetivo transformar as necessidades de explicação em mecanismos explicativos adequados.

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

- **Opcional:**  
  - [Lista de Item de Trabalho](#) 

- **Saídas Intermediárias:**  
  - [Glossário](#)
  - [Lista de Item de Trabalhos](#)
  - [Documento de Requisitos de Explicabilidade - DRE](../artefatos/DRE.md)
---

## Passos
***1. Caracterizar requisitos de explicabilidade***

**O que fazer**

Analisar cada requisito de explicabilidade identificado durante a elicitação para compreender seu contexto de uso e seus objetivos. O propósito desta atividade é obter informações suficientes para apoiar a seleção de mecanismos explicativos adequados e identificar possíveis riscos, conflitos ou limitações.

Para cada requisito, validar:

- Quem necessita da explicação
- Qual o perfil do stakeholder (especialista, usuário final, auditor, gestor, regulador, etc.)
- Qual o objetivo da explicação
- Em qual contexto a explicação será utilizada
- Qual o impacto da decisão apoiada pelo sistema
- Quais requisitos regulatórios, éticos ou organizacionais estão associados.

**Quem**

- Engenheiro de Requisitos (líder), ccom apoio dos Stakeholders, Especialistas de Domínio e Especialistas em IA.

**Onde registrar**

[DRE] - ver onde registrar
Requisitos de Explicabilidade Refinados (RER) - artefato intermediário???Validar

**Boas Práticas**

- Considerar diferentes perfis de stakeholders
- Registrar o contexto de uso da explicação
- Avaliar o impacto da decisão apoiada pelo sistema
- Identificar requisitos regulatórios associados.

  *Perguntas úteis*
- Quem utilizará a explicação?
- Qual decisão está sendo apoiada?
- Qual o risco associado à decisão?
- Qual o objetivo principal da explicação?
- Existe obrigação regulatória para explicar a decisão?


***2. Classificar necessidades explicativas***

**O que fazer**

Classificar os requisitos de acordo com a necessidade explicativa predominante. Essa classificação auxilia na escolha dos mecanismos explicativos mais adequados e facilita a análise posterior.

Exemplo:

- | Necessidade   | Exemplos                |
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

- [DRE] - ver onde registrar
- Requisitos de Explicabilidade Refinados (RER) - artefato intermediário???Validar


**Boas Práticas**

-  Permitir múltiplas classificações para um mesmo requisito quando necessário.
-  Validar a classificação junto aos stakeholders.
-  Evitar assumir que todos os usuários possuem os mesmos objetivos.

 ***3. Mapear para tipos de explicação***

**O que fazer**
Associar cada requisito de explicabilidade a um ou mais tipos de explicação que melhor atendam ao perfil do stakeholder, ao contexto da decisão e ao objetivo da explicação.
O objetivo não é selecionar uma ferramenta específica, mas identificar quais abordagens explicativas possuem maior aderência às necessidades identificadas.


| Necessidade                     | Tipo de Explicação         |
| ------------------------------- | -------------------------- |
| Justificativa clínica           | Feature Importance         |
| Explicar caso específico        | Local Explanation          |
| Explicar comportamento geral    | Global Explanation         |
| Demonstrar exemplos semelhantes | Example-based Explanation  |
| Mostrar regras                  | Rule-based Explanation     |
| Mostrar impacto dos atributos   | Counterfactual Explanation |

**Quem**

Engenheiro de Requisitos

**Onde registrar**

[DRE] - ver onde registrar

**Boas práticas**




---
***4. Analisar conflitos e divergências***

**O que fazer**

- Fazer revisão formal da Visão da Explicabilidade com stakeholders e time técnico; coletar aprovações, feedbacks e registrar decisões.
- Ajustar [Documento de Visão de Explicabilidade](../tarefas/documento-requisito.md), conforme consenso.

**Quem**

Engenheiro de Requisitos (facilitador), Stakeholders, Gerente de Projeto, Arquiteto.

**Onde registrar**

- [Documento de Visão de Explicabilidade](../tarefas/definir-visao.md) (versão aprovada)

**Boas Práticas**

- [](#)


***5. Analisar dependências e restrições***

**O que fazer**

- 

**Quem**

Engenheiro de Requisitos (facilitador), Stakeholders, Gerente de Projeto, Arquiteto.

**Onde registrar**

- [Documento de Visão de Explicabilidade](../tarefas/definir-visao.md) 

**Boas Práticas**

- [VAMOS TER UM DOCUMENTO INDICANDO BOAS PRÁTICAS?](#)

***6. Avaliar viabilidade dos requisitos***

**O que fazer**

- 

**Quem**

Engenheiro de Requisitos (facilitador), Stakeholders, Gerente de Projeto, Arquiteto.

**Onde registrar**

- [Documento de Visão de Explicabilidade](../tarefas/definir-visao.md) 

**Boas Práticas**

- [VAMOS TER UM DOCUMENTO INDICANDO BOAS PRÁTICAS?](#)

***7. Priorizar requisitos usando MoScoW***

**O que fazer**

- 

**Quem**

Engenheiro de Requisitos (facilitador), Stakeholders, Gerente de Projeto, Arquiteto.

**Onde registrar**

- [Documento de Visão de Explicabilidade](../tarefas/definir-visao.md) 

**Boas Práticas**

- [VAMOS TER UM DOCUMENTO INDICANDO BOAS PRÁTICAS?](#)

***8. Obter consenso***

**O que fazer**

- 

**Quem**

Engenheiro de Requisitos (facilitador), Stakeholders, Gerente de Projeto, Arquiteto.

**Onde registrar**

- [Documento de Visão de Explicabilidade](../tarefas/definir-visao.md) 

**Boas Práticas**

- [VAMOS TER UM DOCUMENTO INDICANDO BOAS PRÁTICAS?](#)

---

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
- [Link para o OpenUP Original](file:///C:/Users/Livia%20Mancine/Downloads/OpenUP/Publish/openup/tasks/define_vision_9D36CF2F.html)



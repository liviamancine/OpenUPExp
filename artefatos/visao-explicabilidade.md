# Documento de Visão — Requisito de Explicabilidade
> **Projeto:** *Nome do Projeto*  
> **Data:** dd/mm/aaaa  
> **Versão:** 1.0  

---

## 1. Definição da Explicabilidade
Este documento apresenta uma visão geral do requisito de explicabilidade.

Sugestão:
O problema da falta de explicabilidade em sistemas de Aprendizado de Máquina aplicados a [tarefa/objetivo do sistema] afeta diretamente [categoria de usuários impactados], pois gera [dificuldades ou limitações observadas, como falta de compreensão, perda de confiança, necessidade de transparência].

Uma solução bem-sucedida deve fornecer [tipo de explicações desejadas: técnicas, claras, rastreáveis, contextualizadas, adaptadas ao usuário], permitindo que [usuário ou papel] consiga [ação esperada: entender os critérios utilizados, validar decisões, aumentar confiança, reduzir retrabalho, cumprir normas regulatórias].

---

## 2. Posicionamento

### 2.1 Declaração do Problema
Apresente uma declaração que resuma o problema que este projeto visa resolver. O seguinte formato pode ser utilizado:

| Elemento                     | Descrição                                                                                         |
|------------------------------|---------------------------------------------------------------------------------------------------|
| **O problema da**            | falta de explicabilidade em sistemas de aprendizado de máquina                                    |
| **afeta**                    | Stakeholders impactados: clientes, usuários finais, reguladores, administradores                  |
| **cujo o impacto é**         | descrição das consequências: falta de confiança, barreiras legais, dificuldade de adoção, dificuldade de validação e retrabalho|
| **uma solução bem sucedida seria**| benefícios esperados: transparência, auditoria, aceitação do sistema |

### 2.2 Declaração de Posicionamento da Explicabilidade (fazer para cada perfil de usuário que necessita de explicabilidade)

| Elemento | Descrição |
|----------|-----------|
| **Para quem** | público-alvo do sistema |
| **Para que** | necessitam compreender, auditar ou confiar nas decisões do sistema |
| **O (nome do produto)** | é um(a) *[categoria do produto]* |
| **Benefício principal** | O que o produto faz, seu benefício principal. |
| **Alternativa concorrente** | *[principal alternativa concorrente]* |
| **Diferenciação do produto** | *[principal diferencial do produto]* |

Uma declaração de posicionamento comunica a intenção do produto e sua importância para todos os envolvidos no projeto.

## 3. Descrição dos stakeholders que necessitam de explicabilidade

### 3.1 Resumo dos stakeholders 

descricao - Breve descrição do stakeholder e de sua relação com o sistema e/ou com a explicabilidade, conforme sustentado pelas informações disponíveis.

responsabilidade - Síntese das principais responsabilidades, interesses ou expectativas do stakeholder em relação à explicabilidade do sistema, derivada das informações produzidas pelos Workers anteriores.


| Stakeholders                     | Descrição                                      | Responsabilidade                                        |
|------------------------------|------------------------------------------------|---------------------------------------------------------|
| **Cliente**                  | representa a organização que financia o projeto| Garante que os requisitos de explicabilidade estejam alinhados com metas de negócio|
| **Usuário final**            | interage diretamente com o sistema             | Compreender e confiar nas explicações fornecidas                                   |
| **Regulador**                | Órgão de auditoria ou legislação               | Garantir conformidade legal e ética |


### 3.2 Ambiente do usuário
Descreva como os usuários trabalham e em que situações interagem com as decisões do sistema e com as explicações.

**Exemplos:**
- Em que momento da atividade o usuário recebe a decisão ou recomendação do sistema.
- Se a interação ocorre sob pressão de tempo ou em situações críticas.
- Se o usuário trabalha sozinho ou precisa justificar a decisão a outras pessoas (clientes, gestores, auditores).
- Com que frequência o usuário interage com o sistema.

As plataformas e os ambientes que limitam a solução são registrados na seção 5.2.

## 4. Visão Geral da Explicabilidade 

### 4.1 Necessidades 

Evite detalhes de design. Mantenha as descrições das funcionalidades em um nível geral. Concentre-se nas capacidades necessárias e no porquê (não em como) elas devem ser implementadas. Registre a prioridade das partes interessadas e o lançamento planejado para cada funcionalidade.

| Necessidade                     | Prioridade   |   Planned Release|
|---------------------------------|--------------|-------------------------------------------|
| **Entender decisões do sistema**               | Alta|   Versão 1  |
| **Possibilitar auditoria regulatória**         | Alta |  Versão 1|
| **Explicações ajustadas ao perfil do usuário** | Média | Versão 2|
| **Garantir aderência a normas éticas e legais**| Alta |  Versão 1|


## 5. Restrições da Explicabilidade

Esta seção descreve as restrições que impactam a explicabilidade do sistema: normas e regulamentos aplicáveis, plataformas e ambientes de uso, dependências e assunções. Mantenha as restrições em alto nível; parâmetros detalhados, como tempos de resposta e critérios de qualidade das explicações, são definidos na Especificação.


---

### 5.1 Padrões, Normas e Regulamentos Aplicáveis

Liste normas técnicas, diretrizes regulatórias e regras organizacionais que impactam a explicabilidade.

**Exemplos:**
- Normas de transparência e auditabilidade aplicáveis ao domínio.
- Políticas internas de governança algorítmica.
- Diretrizes éticas que exigem explicações compreensíveis.

---

### 5.2 Plataforma e Ambientes

Descreva as plataformas e os ambientes em que as explicações serão disponibilizadas.

**Exemplos:**
- Plataformas web e desktop.
- Ambientes com baixa conectividade.
- Integração com sistemas já utilizados pelos usuários.

---

### 5.3 Dependências e Assunções

Identifica fatores externos que influenciam a viabilidade da explicabilidade.

**Exemplos:**
- A arquitetura deve permitir o registro de informações para auditoria posterior.
- O módulo de explicabilidade depende da disponibilidade de uma API de inferência estável.

> **Nota:** Se qualquer dependência ou assunção mudar, esta Visão deverá ser revisada.

---

### 5.4 Priorização das Restrições


| Requisito | Prioridade | Planned Release | 
|-----------|------------|--------------|
| Conformidade com normas e regulamentos aplicáveis | Alta | Versão 1 | 
| Operação em plataformas web e desktops | Alta | Versão 1 | 

---
## 6. Definição do Escopo e Limites da Explicabilidade


Especifique até onde a explicabilidade deve chegar, distinguindo os elementos do sistema que exigem explicação daqueles que não fazem parte do requisito.

| Elemento | Descrição |
|----------|-----------|
| **Decisões que requerem explicação** | decisões, recomendações ou previsões do sistema que devem ser explicadas |
| **Stakeholders que recebem explicações** | perfis que receberão explicações (ex.: usuários finais, especialistas de domínio, auditores) |
| **Pontos de interação** | onde a explicação será apresentada (ex.: interface, API, relatórios) |
| **Informações envolvidas** | dados, atributos e resultados do modelo envolvidos no processo explicativo |
| **Fora do escopo** | decisões, módulos ou stakeholders que não serão contemplados |




# 📘 PRDs (Product Requirement Documents) — Fundamentos, Estrutura e Template

Este documento tem como objetivo **explicar os fundamentos de um PRD**, detalhar **sua estrutura ideal**, contextualizar **quando e por que usar**, e apresentar **um template de PRD bem estruturado**, alinhado às boas práticas do mercado.

> Importante:  
> Este material é apenas uma ferramenta de apoio, não uma regra ou  modelo escrito em pedra. 

---

## 1️⃣ O que é um PRD?

O **PRD (Product Requirement Document)** é o documento que descreve **o que deve ser construído e por quê**, do ponto de vista do **produto e do negócio**, servindo como contrato de entendimento entre:

- Produto (PM / PO)
- Engenharia
- Design
- Stakeholders técnicos e não técnicos

O PRD **não descreve código**, mas descreve **comportamento esperado, critérios de sucesso e limites claros**.

---

## 2️⃣ Qual problema o PRD resolve?

Sem PRD:
- Expectativas desalinhadas
- Escopo mutável e implícito
- Decisões tomadas tarde demais
- Discussões recorrentes sobre “o que foi combinado”

Com PRD:
- Clareza de propósito
- Objetivos mensuráveis
- Escopo explícito
- Base sólida para Design Docs, estimativas e execução

---

## 3️⃣ PRD NÃO é

- Documento técnico detalhado
- Arquitetura de software
- Plano de projeto
- Lista de tarefas
- Cronograma

Esses documentos **derivam do PRD**, mas não o substituem.

---

## 4️⃣ Quando usar um PRD?

Use PRD quando:
- Existe impacto em usuários ou negócio
- Há mais de uma pessoa envolvida na entrega
- A feature não é trivial
- O custo de erro é alto
- A decisão precisa ser registrada

Evite PRD formal quando:
- Ajustes muito pequenos
- Correções óbvias e localizadas
- Experimentos extremamente rápidos (spikes)

---

## 5️⃣ Estrutura conceitual de um bom PRD

Um PRD sólido sempre responde a quatro perguntas fundamentais:

### 1. Por que isso existe?
- Contexto
- Problema
- Oportunidade

### 2. O que precisa ser feito?
- Escopo
- Requisitos funcionais
- Requisitos não funcionais

### 3. Como saberemos que deu certo?
- Objetivos
- Métricas
- Critérios de aceitação

### 4. Onde isso vai rodar?
- Sistema alvo
- Contexto de implantação
- Dependências

---

## 6️⃣ Componentes essenciais de um PRD

### 🔹 Contexto e problema
Descreve:
- Produto ou sistema
- Público-alvo
- Cenários de uso
- Problemas reais e priorizados

Boa prática:
- Usar exemplos reais
- Sempre que possível, usar números aproximados

---

### 🔹 Objetivos e métricas
Converte intenção em resultado mensurável.

Estrutura ideal:
- Objetivo → Métrica → Meta alvo

Exemplo:
- Objetivo: reduzir abandono
- Métrica: taxa de conversão
- Meta: +15% em 90 dias

---

### 🔹 Escopo
Define limites claros.

- **Dentro do escopo**: o que obrigatoriamente será entregue
- **Fora do escopo**: o que explicitamente não será feito

Essa seção reduz conflitos futuros.

---

### 🔹 Requisitos funcionais
Descrevem **o comportamento do sistema**.

Cada requisito funcional bem escrito possui:
- Nome claro
- Descrição objetiva
- Fluxo principal
- Fluxos alternativos e exceções
- Erros previstos
- Prioridade

---

### 🔹 Requisitos não funcionais
Definem **qualidade, limites e garantias** do sistema.

Categorias comuns:
- Performance
- Disponibilidade
- Segurança
- Observabilidade
- Confiabilidade
- Compliance
- Acessibilidade

Sempre que possível, devem conter **números ou critérios verificáveis**.

---

### 🔹 Arquitetura e abordagem (nível de PRD)
No PRD, arquitetura aparece **em nível conceitual**, não em detalhe técnico profundo.

Exemplos:
- Tipo de sistema (monólito, microsserviço, agente de IA)
- Tipo de comunicação
- Integrações relevantes
- Restrições técnicas já conhecidas

---

### 🔹 Decisões e trade-offs
Registra decisões já tomadas e seus custos.

Formato recomendado:
- Decisão
- Justificativa
- Trade-off

---

### 🔹 Dependências
Tudo que **não está sob controle direto** da feature.

Tipos comuns:
- Técnicas
- Organizacionais
- Externas

---

### 🔹 Riscos e mitigação
Antecipação estruturada de problemas.

Cada risco deve ter:
- Probabilidade
- Impacto
- Mitigações (pode haver várias)
- Plano de contingência

---

### 🔹 Critérios de aceitação
Checklist objetivo que define “pronto”.

Boa prática:
- Frases verificáveis
- Sem subjetividade
- Usáveis como base para QA

---

### 🔹 Testes e validação
Define como a feature será validada antes de ir para produção.

Inclui:
- Tipos de teste obrigatórios
- Estratégia geral de validação

---

## 7️⃣ Template base de PRD (para estudos)

```markdown
### PRD: [Produto] [Feature]

Versão:
Data:
Responsável:

---

### Resumo
[Visão geral da feature e seu propósito]

---

### Contexto e problema
[Público-alvo, cenários de uso e problemas priorizados]

---

### Objetivos e métricas
| Objetivo | Métrica | Meta |

---

### Escopo
Incluso
- ...

Fora de escopo
- ...

---

### Requisitos funcionais
#### [ID] [Nome]
- Descrição
- Fluxo principal
- Fluxos alternativos
- Erros previstos
- Prioridade

---

### Requisitos não funcionais
- Performance
- Disponibilidade
- Segurança
- Observabilidade
- Outros

---

### Arquitetura e abordagem
- Visão geral
- Componentes
- Integrações

---

### Decisões e trade-offs
- Decisão
- Justificativa
- Trade-off

---

### Dependências
- Tipo
- Descrição

---

### Riscos e mitigação
- Risco
- Probabilidade
- Impacto
- Mitigação
- Contingência

---

### Critérios de aceitação
- Checklist objetivo

---

### Testes e validação
- Tipos de teste
- Estratégia

## 8️⃣ Relação entre PRD e outros documentos
PRD
 ↓
Design Doc
 ↓
ADRs
 ↓
Implementação


- PRD define o que

- Design Doc define como

- ADR registra decisões

- Código executa
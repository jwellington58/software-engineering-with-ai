# 📘 Design Docs em Engenharia de Software (com IA)

Este documento apresenta uma visão **estrutural e prática** sobre **Design Docs**, seus principais tipos usados no mercado, quando utilizá-los e como eles se relacionam com **PRDs (Product Requirement Documents)**.  
O objetivo é servir como **material de estudo e consulta** ao longo do MBA e na prática profissional.

---

## 1️⃣ O que são Design Docs?

**Design Docs (Documentos de Design)** são documentos técnicos criados **antes da implementação**, cujo objetivo é descrever **como uma solução será projetada**, quais decisões serão tomadas e quais trade-offs estão envolvidos.

Eles respondem perguntas como:
- O que será construído?
- Por que essa solução é necessária?
- Como ela será implementada?
- Quais alternativas foram consideradas?
- Quais riscos e impactos existem?

> **Ideia central:** Design Docs ajudam a pensar, alinhar e decidir **antes do código existir**.

---

## 2️⃣ Por que Design Docs são importantes?

### Benefícios principais
- Alinhamento técnico entre times
- Decisões explícitas e registradas
- Redução de retrabalho
- Facilita revisões e feedback
- Escala o conhecimento do time
- Ajuda no onboarding
- Cria histórico técnico do sistema

### O que acontece sem Design Docs
- Decisões implícitas
- Arquitetura caótica
- Dependência de pessoas específicas
- Dificuldade de manutenção
- Conflitos técnicos recorrentes

---

## 3️⃣ Design Docs x Documentação Final

| Design Doc | Documentação Final |
|-----------|-------------------|
| Antes do código | Depois do código |
| Foco em decisões | Foco em uso |
| Explora alternativas | Explica implementação |
| Pode mudar | Representa o estado atual |

---

## 4️⃣ Tipos de Design Docs mais usados no mercado

---

## 🔹 4.1 One-Pager Design Doc

### O que é
Documento curto (1–2 páginas) para descrever uma solução de forma objetiva.

### Conteúdo típico
- Contexto
- Problema
- Solução proposta
- Impactos
- Riscos

### Quando usar
- Features pequenas
- MVPs
- Times pequenos
- Decisões rápidas

### Quando não usar
- Mudanças arquiteturais grandes
- Sistemas críticos

---

## 🔹 4.2 Technical Design Document (TDD)

### O que é
Documento técnico detalhado que descreve **como a solução será implementada**.

### Conteúdo típico
- Arquitetura
- Diagramas
- Fluxos
- APIs
- Banco de dados
- Segurança
- Performance

### Quando usar
- Funcionalidades médias ou grandes
- Integrações
- Quando múltiplos times implementam

---

## 🔹 4.3 Architecture Design Document (ADD)

### O que é
Documento focado na **arquitetura do sistema como um todo**.

### Conteúdo típico
- Visão geral
- Componentes
- Comunicação
- Padrões arquiteturais
- Trade-offs
- Diagramas (C4, UML)

### Quando usar
- Novo sistema
- Reescrita
- Migração
- Escalabilidade

---

## 🔹 4.4 RFC (Request for Comments)

### O que é
Documento para **propor mudanças** e coletar feedback técnico.

### Conteúdo típico
- Motivação
- Proposta
- Alternativas
- Impactos
- Questões abertas

### Quando usar
- Mudanças que afetam vários times
- Padrões internos
- Decisões polêmicas

---

## 🔹 4.5 ADR (Architecture Decision Record)

### O que é
Documento curto que registra **uma decisão arquitetural específica**.

### Conteúdo típico
- Contexto
- Decisão
- Alternativas consideradas
- Consequências

### Quando usar
- Sempre que uma decisão arquitetural relevante for tomada

---

## 🔹 4.6 Design Doc para IA / ML / LLM

### O que é
Documento especializado para sistemas de IA.

### Conteúdo típico
- Objetivo do modelo
- Dados
- Prompting / RAG
- Métricas
- Riscos éticos
- Observabilidade
- Feedback loop

### Quando usar
- IA em produção
- Sistemas de agentes
- Decisões automatizadas

---

## 5️⃣ Quando usar cada tipo (resumo)

| Situação | Documento |
|--------|----------|
| Feature pequena | One-Pager |
| Feature média/grande | TDD |
| Novo sistema | ADD |
| Mudança transversal | RFC |
| Decisão arquitetural | ADR |
| Sistemas de IA | Design Doc de IA |

---

## 6️⃣ Onde a IA entra nos Design Docs?

A IA pode ajudar a:
- gerar rascunhos iniciais
- comparar alternativas
- identificar riscos
- revisar inconsistências
- padronizar templates
- explicar decisões para públicos não técnicos

> **Importante:** IA apoia a decisão, mas não substitui o julgamento humano.

---

# 🔸 EXTRA — PRD (Product Requirement Document)

## O que é um PRD?

O **PRD (Product Requirement Document)** descreve **o que deve ser construído do ponto de vista do produto**, não da implementação técnica.

Ele foca em:
- problema do usuário
- objetivos de negócio
- requisitos funcionais
- requisitos não funcionais
- critérios de sucesso

> **PRD define o “O QUÊ” e o “POR QUÊ”**  
> **Design Doc define o “COMO”**

---

## Conteúdo típico de um PRD

- Visão do produto
- Problema a ser resolvido
- Personas / usuários
- Requisitos funcionais
- Requisitos não funcionais
- Casos de uso
- Métricas de sucesso
- Fora de escopo
- Restrições

---

## PRD x Design Doc

| PRD | Design Doc |
|---|---|
| Foco no produto | Foco técnico |
| Linguagem mais acessível | Linguagem técnica |
| Define requisitos | Define solução |
| Escrito por PM / PO | Escrito por engenheiros |
| Vem antes | Vem depois |

---

## Fluxo típico no mercado

- PRD → Design Doc → Implementação → Documentação Final


Em times maduros:
- PRD e Design Doc se complementam
- Mudanças no PRD geram revisões no Design Doc
- ADRs registram decisões tomadas durante o design

---

## 7️⃣ Conclusão

- Design Docs são ferramentas de **pensamento e alinhamento**
- Não são burocracia, são aceleradores
- O tipo certo depende do contexto
- PRDs definem o problema, Design Docs resolvem o problema
- IA potencializa a criação e revisão desses documentos

---

## 📚 Sugestões para aprofundar

- Criar templates reutilizáveis
- Versionar Design Docs em repositório
- Associar ADRs a PRDs
- Usar IA para revisão e geração de alternativas
- Integrar Design Docs ao fluxo de desenvolvimento

---
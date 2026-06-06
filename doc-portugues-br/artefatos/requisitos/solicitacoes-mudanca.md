# Solicitações de Mudança

## Objetivo

Este documento registra solicitações de mudança relacionadas ao projeto, permitindo rastrear alterações de requisitos, arquitetura, processos, cronograma ou escopo.

O objetivo é garantir que toda alteração relevante seja analisada, aprovada e documentada antes de sua implementação.

---

# Processo de Mudança

Fluxo padrão:

```text
Solicitação
      ↓
Análise de Impacto
      ↓
Aprovação
      ↓
Planejamento
      ↓
Implementação
      ↓
Testes
      ↓
Release
```

---

# Status Possíveis

| Status       | Descrição                          |
| ------------ | ---------------------------------- |
| Aberta       | Solicitação registrada             |
| Em Análise   | Avaliação de impacto em andamento  |
| Aprovada     | Mudança aprovada                   |
| Rejeitada    | Mudança recusada                   |
| Implementada | Alteração concluída                |
| Cancelada    | Solicitação encerrada sem execução |

---

# Critérios de Avaliação

Toda solicitação deverá avaliar:

* Impacto no escopo;
* Impacto no prazo;
* Impacto na arquitetura;
* Impacto na qualidade;
* Impacto na segurança;
* Impacto nos testes;
* Impacto nos custos.

---

# Registro de Solicitações

## SM-001

### Informações Gerais

| Campo               | Valor         |
| ------------------- | ------------- |
| ID                  | SM-001        |
| Data da Solicitação | 10/06/2026    |
| Solicitante         | Product Owner |
| Status              | Implementada  |
| Prioridade          | Alta          |

### Descrição

Adicionar funcionalidade de recuperação de senha por e-mail.

### Justificativa

Usuários não possuem mecanismo para recuperar acesso à plataforma.

### Análise de Impacto

| Área           | Impacto |
| -------------- | ------- |
| Backend        | Médio   |
| Flutter        | Médio   |
| Angular        | Médio   |
| Banco de Dados | Baixo   |
| Testes         | Médio   |

### Requisitos Afetados

* REQ-F-003

### Casos de Teste Afetados

* CT-008
* CT-009

### Decisão

Aprovada.

### Responsável

Stephanye Castellano

### Data de Implementação

20/06/2026

### Observações

Funcionalidade entregue na Release 0.1.0.

---

## SM-002

### Informações Gerais

| Campo               | Valor          |
| ------------------- | -------------- |
| ID                  | SM-002         |
| Data da Solicitação | 25/06/2026     |
| Solicitante         | Equipe Técnica |
| Status              | Aprovada       |
| Prioridade          | Média          |

### Descrição

Substituir autenticação simples por autenticação JWT.

### Justificativa

Melhorar segurança e compatibilidade entre aplicações.

### Análise de Impacto

| Área           | Impacto |
| -------------- | ------- |
| Backend        | Alto    |
| Flutter        | Médio   |
| Angular        | Médio   |
| Banco de Dados | Baixo   |
| Testes         | Alto    |

### Requisitos Afetados

* RNF-001
* RNF-002

### Casos de Teste Afetados

* CT-010
* CT-011
* CT-012

### Decisão

Aprovada.

### Responsável

Equipe de Desenvolvimento

### Data Prevista

15/07/2026

### Observações

Necessário atualizar documentação de arquitetura.

---

## SM-003

### Informações Gerais

| Campo               | Valor         |
| ------------------- | ------------- |
| ID                  | SM-003        |
| Data da Solicitação | 01/07/2026    |
| Solicitante         | Usuário Final |
| Status              | Rejeitada     |
| Prioridade          | Baixa         |

### Descrição

Adicionar tema personalizado para cada usuário.

### Justificativa

Melhorar experiência visual.

### Análise de Impacto

| Área           | Impacto |
| -------------- | ------- |
| Backend        | Baixo   |
| Flutter        | Médio   |
| Angular        | Médio   |
| Banco de Dados | Baixo   |
| Testes         | Médio   |

### Motivo da Rejeição

Funcionalidade fora do escopo atual do produto.

### Observações

Poderá ser reavaliada em versões futuras.

---

# Template para Nova Solicitação

## SM-XXX

### Informações Gerais

| Campo               | Valor |
| ------------------- | ----- |
| ID                  |       |
| Data da Solicitação |       |
| Solicitante         |       |
| Status              |       |
| Prioridade          |       |

### Descrição

Descrever a mudança solicitada.

### Justificativa

Motivo da solicitação.

### Análise de Impacto

| Área           | Impacto |
| -------------- | ------- |
| Backend        |         |
| Flutter        |         |
| Angular        |         |
| Banco de Dados |         |
| Testes         |         |

### Requisitos Afetados

* REQ-XXX

### Casos de Teste Afetados

* CT-XXX

### Rastreabilidade da Mudança

| Artefato | Identificador |
|-----------|-----------|
| Solicitação de Mudança | SM-002 |
| Requisitos Relacionados | RNF-001, RNF-002 |
| Casos de Teste Relacionados | CT-010, CT-011, CT-012 |
| Decisão Arquitetural Relacionada | ADR-006 |
| Release Relacionada | 0.2.0 |

### Decisão

Aprovada / Rejeitada

### Responsável

Nome do responsável.

### Data Prevista

DD/MM/AAAA

### Observações

Informações adicionais.

---

# Indicadores

As seguintes métricas poderão ser acompanhadas:

| Indicador                    | Objetivo               |
| ---------------------------- | ---------------------- |
| Solicitações abertas         | Controle de demanda    |
| Solicitações aprovadas       | Evolução do produto    |
| Solicitações rejeitadas      | Controle de escopo     |
| Tempo médio de aprovação     | Eficiência do processo |
| Tempo médio de implementação | Produtividade          |

---

# Histórico de Alterações

| Data       | Versão | Descrição                    |
| ---------- | ------ | ---------------------------- |
| 04/06/2026 | 1.0    | Criação inicial do documento |

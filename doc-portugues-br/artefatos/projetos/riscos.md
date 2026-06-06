# Gestão de Riscos

## Objetivo

Este documento tem como objetivo identificar, avaliar, monitorar e mitigar riscos que possam impactar o desenvolvimento, a qualidade, o prazo, o custo ou a operação do sistema.

A gestão de riscos deve ser realizada continuamente durante todo o ciclo de vida do projeto.

---

# Critérios de Avaliação

## Impacto

| Nível   | Descrição                                         |
| ------- | ------------------------------------------------- |
| Baixo   | Pequeno impacto no projeto                        |
| Médio   | Impacto moderado em prazo, qualidade ou escopo    |
| Alto    | Impacto significativo no projeto                  |
| Crítico | Pode comprometer a entrega ou operação do sistema |

---

## Probabilidade

| Nível | Descrição              |
| ----- | ---------------------- |
| Baixa | Pouco provável         |
| Média | Pode ocorrer           |
| Alta  | Alta chance de ocorrer |

---

# Classificação do Risco

A prioridade do risco deve considerar a combinação entre impacto e probabilidade.

| Impacto | Probabilidade | Prioridade |
| ------- | ------------- | ---------- |
| Baixo   | Baixa         | Baixa      |
| Médio   | Baixa         | Baixa      |
| Médio   | Média         | Média      |
| Alto    | Média         | Alta       |
| Alto    | Alta          | Crítica    |
| Crítico | Alta          | Crítica    |

---

# Registro de Riscos

## RSK-001

### Informações

| Campo      | Valor        |
| ---------- | ------------ |
| ID         | RSK-001      |
| Categoria  | Planejamento |
| Status     | Aberto       |
| Prioridade | Alta         |

### Descrição

Atraso no desenvolvimento devido à execução do projeto por uma única pessoa.

### Impacto

Alto

### Probabilidade

Alta

### Mitigação

* Priorizar funcionalidades do MVP.
* Manter backlog organizado.
* Evitar iniciar múltiplas funcionalidades simultaneamente.

### Plano de Contingência

Reduzir escopo da release e replanejar entregas.

---

## RSK-002

### Informações

| Campo      | Valor      |
| ---------- | ---------- |
| ID         | RSK-002    |
| Categoria  | Tecnologia |
| Status     | Aberto     |
| Prioridade | Média      |

### Descrição

Mudanças de requisitos durante o desenvolvimento.

### Impacto

Médio

### Probabilidade

Alta

### Mitigação

* Formalizar requisitos antes da implementação.
* Utilizar critérios de aceitação.
* Registrar alterações em documentos de requisitos.

### Plano de Contingência

Reavaliar cronograma e atualizar documentação.

---

## RSK-003

### Informações

| Campo      | Valor      |
| ---------- | ---------- |
| ID         | RSK-003    |
| Categoria  | Integração |
| Status     | Aberto     |
| Prioridade | Alta       |

### Descrição

Falhas na integração entre aplicações frontend e backend.

### Impacto

Alto

### Probabilidade

Média

### Mitigação

* Criar contratos claros para APIs.
* Utilizar Swagger/OpenAPI.
* Executar testes de integração regularmente.

### Plano de Contingência

Correção imediata das integrações impactadas.

---

## RSK-004

### Informações

| Campo      | Valor     |
| ---------- | --------- |
| ID         | RSK-004   |
| Categoria  | Qualidade |
| Status     | Aberto    |
| Prioridade | Alta      |

### Descrição

Defeitos não identificados antes da publicação.

### Impacto

Alto

### Probabilidade

Média

### Mitigação

* Executar testes unitários.
* Executar testes de integração.
* Executar testes exploratórios.
* Utilizar checklist de release.

### Plano de Contingência

Publicar correção emergencial (hotfix).

---

## RSK-005

### Informações

| Campo      | Valor          |
| ---------- | -------------- |
| ID         | RSK-005        |
| Categoria  | Infraestrutura |
| Status     | Aberto         |
| Prioridade | Média          |

### Descrição

Perda de código ou documentação.

### Impacto

Alto

### Probabilidade

Baixa

### Mitigação

* Utilizar GitHub.
* Realizar commits frequentes.
* Manter documentação versionada.

### Plano de Contingência

Recuperação através do histórico do repositório.

---

## RSK-006

### Informações

| Campo      | Valor     |
| ---------- | --------- |
| ID         | RSK-006   |
| Categoria  | Segurança |
| Status     | Aberto    |
| Prioridade | Crítica   |

### Descrição

Exposição de dados sensíveis de usuários.

### Impacto

Crítico

### Probabilidade

Média

### Mitigação

* Utilizar HTTPS.
* Utilizar autenticação JWT.
* Validar entradas.
* Aplicar boas práticas de segurança.

### Plano de Contingência

Bloqueio imediato da vulnerabilidade e comunicação aos usuários afetados.

---

# Riscos Encerrados

## RSK-000

### Descrição

Escolha da stack tecnológica.

### Status

Encerrado.

### Resolução

Definidas as tecnologias:

* Backend: .NET
* Frontend Mobile/Desktop: Flutter
* Frontend Web: Angular

---

# Monitoramento

Os riscos deverão ser revisados:

* A cada nova release.
* Quando houver alteração significativa de escopo.
* Quando um risco for materializado.
* Durante revisões de planejamento.

---

# Template para Novos Riscos

## RSK-XXX

### Informações

| Campo      | Valor |
| ---------- | ----- |
| ID         |       |
| Categoria  |       |
| Status     |       |
| Prioridade |       |

### Descrição

Descrever o risco.

### Impacto

Baixo / Médio / Alto / Crítico

### Probabilidade

Baixa / Média / Alta

### Mitigação

Ações para reduzir a probabilidade ou impacto.

### Plano de Contingência

Ações a serem executadas caso o risco ocorra.

---

# Histórico de Alterações

| Data       | Versão | Descrição                    |
| ---------- | ------ | ---------------------------- |
| 04/06/2026 | 1.0    | Criação inicial do documento |

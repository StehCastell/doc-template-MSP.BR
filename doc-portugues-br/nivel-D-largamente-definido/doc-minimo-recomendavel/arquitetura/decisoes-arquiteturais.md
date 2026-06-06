# Decisões Arquiteturais

## Objetivo

Este documento registra as principais decisões arquiteturais adotadas durante o desenvolvimento do sistema.

O registro das decisões permite:

- Entender o motivo das escolhas realizadas.
- Facilitar a manutenção futura.
- Apoiar a entrada de novos colaboradores.
- Evitar rediscussões de decisões já tomadas.
- Garantir rastreabilidade técnica.

---

# Como Registrar uma Decisão

Cada decisão arquitetural deve conter:

| Campo | Descrição |
|---------|---------|
| ID | Identificador único |
| Data | Data da decisão |
| Status | Proposta, Aprovada ou Substituída |
| Contexto | Problema ou necessidade |
| Decisão | Solução escolhida |
| Justificativa | Motivos da escolha |
| Consequências | Impactos positivos e negativos |

---

# ADR-001

## Informações

| Campo | Valor |
|---------|---------|
| ID | ADR-001 |
| Data | 04/06/2026 |
| Status | Aprovada |

### Título

Utilizar Flutter para aplicações Mobile e Desktop.

### Contexto

O projeto necessita disponibilizar aplicações para dispositivos móveis e desktop.

Uma das preocupações é reduzir o custo de manutenção e evitar múltiplas bases de código.

### Decisão

Utilizar Flutter para desenvolvimento Mobile e Desktop.

### Justificativa

- Compartilhamento de código.
- Menor esforço de manutenção.
- Ecossistema consolidado.
- Boa performance.
- Facilidade para equipes pequenas.

### Consequências

#### Positivas

- Menor custo de desenvolvimento.
- Reutilização de componentes.
- Estratégia de testes unificada.

#### Negativas

- Dependência do ecossistema Flutter.
- Algumas integrações específicas podem exigir código nativo.

---

# ADR-002

## Informações

| Campo | Valor |
|---------|---------|
| ID | ADR-002 |
| Data | 04/06/2026 |
| Status | Aprovada |

### Título

Utilizar Angular para aplicação Web.

### Contexto

A aplicação Web deverá suportar crescimento futuro e funcionalidades administrativas.

### Decisão

Utilizar Angular como framework frontend.

### Justificativa

- Estrutura robusta.
- Organização modular.
- Forte adoção corporativa.
- Excelente integração com TypeScript.

### Consequências

#### Positivas

- Melhor organização do projeto.
- Facilidade de manutenção.
- Escalabilidade.

#### Negativas

- Curva de aprendizado maior.
- Maior quantidade de configuração inicial.

---

# ADR-003

## Informações

| Campo | Valor |
|---------|---------|
| ID | ADR-003 |
| Data | 04/06/2026 |
| Status | Aprovada |

### Título

Utilizar .NET como plataforma Backend.

### Contexto

O sistema necessita de uma API robusta para atender múltiplos clientes.

### Decisão

Utilizar ASP.NET Core Web API.

### Justificativa

- Excelente desempenho.
- Forte suporte corporativo.
- Ecossistema maduro.
- Ótima integração com testes automatizados.

### Consequências

#### Positivas

- Escalabilidade.
- Facilidade de manutenção.
- Grande disponibilidade de bibliotecas.

#### Negativas

- Hospedagem pode ser mais cara dependendo do ambiente.

---

# ADR-004

## Informações

| Campo | Valor |
|---------|---------|
| ID | ADR-004 |
| Data | 04/06/2026 |
| Status | Aprovada |

### Título

Adotar Clean Architecture no Backend.

### Contexto

O sistema deverá crescer ao longo do tempo e manter boa organização.

### Decisão

Implementar Backend seguindo princípios da Clean Architecture.

### Justificativa

- Separação de responsabilidades.
- Facilidade para testes.
- Maior desacoplamento.

### Consequências

#### Positivas

- Código mais organizado.
- Melhor manutenção.
- Maior facilidade para evolução.

#### Negativas

- Estrutura inicial mais complexa.

---

# ADR-005

## Informações

| Campo | Valor |
|---------|---------|
| ID | ADR-005 |
| Data | 04/06/2026 |
| Status | Aprovada |

### Título

Utilizar arquitetura Feature First no Frontend.

### Contexto

Organizar o sistema por camadas tende a gerar estruturas muito grandes conforme o projeto cresce.

### Decisão

Organizar Angular e Flutter por funcionalidades.

### Justificativa

Estrutura baseada em domínio de negócio:

```text
features
├── auth
├── usuarios
├── pedidos
└── dashboard
```

### Consequências

#### Positivas

- Melhor organização.
- Facilidade de localização de código.
- Escalabilidade.

#### Negativas

- Pode gerar duplicação se não houver padronização.

---

# ADR-006

## Informações

| Campo | Valor |
|---------|---------|
| ID | ADR-006 |
| Data | 04/06/2026 |
| Status | Aprovada |

### Título

Utilizar JWT para autenticação.

### Contexto

A API será consumida por múltiplos clientes.

### Decisão

Implementar autenticação baseada em JWT.

### Justificativa

- Padrão amplamente adotado.
- Compatível com Web, Mobile e Desktop.
- Fácil integração.

### Consequências

#### Positivas

- Arquitetura stateless.
- Escalabilidade.

#### Negativas

- Necessidade de controle de expiração e renovação de tokens.

---

# ADR-007

## Informações

| Campo | Valor |
|---------|---------|
| ID | ADR-007 |
| Data | 04/06/2026 |
| Status | Aprovada |

### Título

Utilizar Monorepositório.

### Contexto

O projeto será inicialmente desenvolvido por uma única pessoa.

### Decisão

Manter Backend, Frontend e Documentação no mesmo repositório.

### Justificativa

```text
Projeto
├── Backend
├── Frontend
├── Documentacao
└── Infraestrutura
```

### Consequências

#### Positivas

- Gestão simplificada.
- Versionamento centralizado.
- Menor esforço operacional.

#### Negativas

- Repositório tende a crescer ao longo do tempo.

---

# ADR-008

## Informações

| Campo | Valor |
|---------|---------|
| ID | ADR-008 |
| Data | 04/06/2026 |
| Status | Aprovada |

### Título

Não utilizar Docker inicialmente.

### Contexto

O projeto será desenvolvido e mantido por uma única pessoa.

### Decisão

Executar aplicações diretamente no ambiente de desenvolvimento durante as fases iniciais.

### Justificativa

- Redução da complexidade operacional.
- Menor curva de aprendizado.
- Agilidade para início do projeto.

### Consequências

#### Positivas

- Menor esforço de configuração.
- Ambiente mais simples.

#### Negativas

- Menor padronização entre ambientes.
- Docker poderá ser necessário futuramente.

---

# Histórico de Alterações

| Data | Versão | Descrição |
|---------|---------|---------|
| 04/06/2026 | 1.0 | Criação inicial do documento |

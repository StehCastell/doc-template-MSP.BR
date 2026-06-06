# Requisitos Não Funcionais

## Objetivo

Este documento descreve os requisitos não funcionais do sistema, estabelecendo critérios de qualidade, desempenho, segurança, usabilidade, compatibilidade e manutenção.

Os requisitos não funcionais definem **como o sistema deve operar**, complementando os requisitos funcionais que definem **o que o sistema deve fazer**.

Cada requisito possui um identificador único para permitir rastreabilidade durante o desenvolvimento e testes.

---

# Convenções

## Prioridade

| Nível | Descrição                                |
| ----- | ---------------------------------------- |
| Alta  | Essencial para operação do sistema       |
| Média | Importante para experiência e manutenção |
| Baixa | Desejável, porém não crítica             |

## Status

| Status           | Descrição                               |
| ---------------- | --------------------------------------- |
| Planejado        | Requisito aprovado para desenvolvimento |
| Em Implementação | Em processo de atendimento              |
| Validado         | Atendido e testado                      |
| Cancelado        | Removido do escopo                      |

---

# Requisitos Não Funcionais

## RNF-001 - Segurança de Autenticação

### Descrição

O sistema deverá proteger o acesso dos usuários através de autenticação segura.

### Prioridade

Alta

### Status

Planejado

### Critérios

* As senhas não deverão ser armazenadas em texto puro.
* As senhas deverão ser armazenadas utilizando algoritmos seguros de hash.
* O acesso às áreas protegidas deverá exigir autenticação válida.
* Sessões expiradas deverão exigir novo login.

---

## RNF-002 - Tempo de Resposta

### Descrição

O sistema deverá responder às operações comuns dentro de um tempo aceitável para o usuário.

### Prioridade

Alta

### Status

Planejado

### Critérios

* Operações de consulta deverão responder em até 3 segundos em condições normais.
* Operações de autenticação deverão responder em até 5 segundos.
* O sistema deverá exibir indicadores de carregamento para operações demoradas.

---

## RNF-003 - Disponibilidade

### Descrição

O sistema deverá permanecer disponível para utilização sempre que possível.

### Prioridade

Alta

### Status

Planejado

### Critérios

* O sistema deverá ser projetado para minimizar indisponibilidades.
* Falhas críticas deverão ser registradas para análise posterior.
* O sistema deverá possuir mecanismos de recuperação de erros quando aplicável.

---

## RNF-004 - Compatibilidade

### Descrição

O sistema deverá funcionar nas plataformas suportadas pelo projeto.

### Prioridade

Alta

### Status

Planejado

### Critérios

#### Aplicação Web

* Compatível com Google Chrome.
* Compatível com Microsoft Edge.
* Compatível com Mozilla Firefox.

#### Aplicação Mobile

* Compatível com Android.
* Compatível com iOS.

#### Aplicação Desktop

* Compatível com Windows.

---

## RNF-005 - Usabilidade

### Descrição

O sistema deverá oferecer uma interface intuitiva e consistente.

### Prioridade

Média

### Status

Planejado

### Critérios

* Os fluxos principais deverão exigir o menor número possível de ações.
* Mensagens de erro deverão ser claras e compreensíveis.
* Elementos visuais deverão manter consistência entre telas.
* O usuário deverá receber feedback visual para ações executadas.

---

## RNF-006 - Manutenibilidade

### Descrição

O sistema deverá ser desenvolvido de forma a facilitar futuras evoluções e correções.

### Prioridade

Alta

### Status

Planejado

### Critérios

* O código deverá seguir padrões definidos pela equipe.
* As funcionalidades deverão possuir testes automatizados.
* A arquitetura deverá favorecer separação de responsabilidades.
* A documentação deverá ser mantida atualizada.

---

## RNF-007 - Testabilidade

### Descrição

O sistema deverá permitir validação eficiente através de testes automatizados e manuais.

### Prioridade

Alta

### Status

Planejado

### Critérios

* Regras de negócio deverão ser desacopladas da interface.
* Componentes deverão permitir testes isolados.
* Funcionalidades críticas deverão possuir cobertura de testes.
* Casos de teste deverão ser rastreáveis aos requisitos.

---

## RNF-008 - Registro de Logs

### Descrição

O sistema deverá registrar eventos relevantes para auditoria e diagnóstico.

### Prioridade

Média

### Status

Planejado

### Critérios

* Erros deverão ser registrados.
* Falhas de autenticação deverão ser registradas.
* Eventos críticos deverão possuir informações suficientes para investigação.
* Informações sensíveis não deverão ser registradas em logs.

---

## RNF-009 - Escalabilidade

### Descrição

A arquitetura deverá permitir crescimento gradual do sistema.

### Prioridade

Média

### Status

Planejado

### Critérios

* Novos módulos poderão ser adicionados sem impacto significativo nos módulos existentes.
* A arquitetura deverá favorecer modularização.
* O sistema deverá permitir evolução para múltiplos usuários simultâneos.

---

## RNF-010 - Backup e Recuperação

### Descrição

Os dados do sistema deverão possuir mecanismos de proteção contra perda.

### Prioridade

Alta

### Status

Planejado

### Critérios

* Os dados deverão possuir estratégia de backup definida.
* O processo de restauração deverá ser documentado.
* Falhas de armazenamento deverão ser identificáveis.

---

# Categorias de Requisitos Não Funcionais

| Categoria            | Identificadores |
| -------------------- | --------------- |
| Segurança            | RNF-001         |
| Desempenho           | RNF-002         |
| Disponibilidade      | RNF-003         |
| Compatibilidade      | RNF-004         |
| Usabilidade          | RNF-005         |
| Manutenibilidade     | RNF-006         |
| Testabilidade        | RNF-007         |
| Auditoria e Logs     | RNF-008         |
| Escalabilidade       | RNF-009         |
| Backup e Recuperação | RNF-010         |

---

# Rastreabilidade

Os requisitos não funcionais deverão possuir vínculo com:

* Casos de teste;
* Métricas de qualidade;
* Arquitetura do sistema;
* Estratégia de testes.

Exemplo:

| Requisito | Caso de Teste | Evidência             |
| --------- | ------------- | --------------------- |
| RNF-001   | CT-SEG-001    | Teste de autenticação |
| RNF-002   | CT-PERF-001   | Teste de desempenho   |
| RNF-007   | CT-QA-001     | Cobertura de testes   |

---

# Histórico de Alterações

| Data       | Versão | Descrição                    |
| ---------- | ------ | ---------------------------- |
| 04/06/2026 | 1.0    | Criação inicial do documento |

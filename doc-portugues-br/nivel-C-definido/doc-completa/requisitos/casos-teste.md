# Casos de Teste

## Objetivo

Este documento tem como objetivo definir os casos de teste utilizados para verificar e validar os requisitos do sistema.

Os casos de teste garantem que as funcionalidades implementadas atendam aos requisitos funcionais e não funcionais definidos, além de fornecer rastreabilidade entre requisitos, implementação e validação.

---

# Convenções

## Identificação

Os casos de teste deverão seguir o padrão:

```text
CT-XXX
```

Exemplos:

```text
CT-001
CT-002
CT-003
```

Casos específicos podem utilizar prefixos por categoria:

```text
CT-FUNC-001  → Funcional
CT-INT-001   → Integração
CT-E2E-001   → Ponta a Ponta
CT-SEG-001   → Segurança
CT-PERF-001  → Desempenho
```

---

# Template de Caso de Teste

| Campo              | Descrição                                         |
| ------------------ | ------------------------------------------------- |
| ID                 | Identificador único                               |
| Requisito          | Requisito associado                               |
| Título             | Nome resumido do teste                            |
| Tipo               | Funcional, Integração, E2E, Segurança, Desempenho |
| Prioridade         | Alta, Média ou Baixa                              |
| Pré-condições      | Condições necessárias                             |
| Passos             | Sequência de execução                             |
| Resultado Esperado | Resultado correto                                 |
| Status             | Não Executado, Aprovado, Reprovado                |

---

# Casos de Teste Funcionais

## CT-FUNC-001 - Cadastro de Usuário com Dados Válidos

### Requisito

REQ-001 - Cadastro de Usuário

### Tipo

Funcional

### Prioridade

Alta

### Pré-condições

* Usuário não cadastrado anteriormente.

### Passos

1. Acessar a tela de cadastro.
2. Informar nome válido.
3. Informar e-mail válido.
4. Informar senha válida.
5. Confirmar cadastro.

### Resultado Esperado

* Conta criada com sucesso.
* Usuário recebe mensagem de confirmação.

### Status

Não Executado

---

## CT-FUNC-002 - Cadastro com E-mail Já Existente

### Requisito

REQ-001 - Cadastro de Usuário

### Tipo

Funcional

### Prioridade

Alta

### Pré-condições

* E-mail já cadastrado no sistema.

### Passos

1. Acessar a tela de cadastro.
2. Informar e-mail já existente.
3. Confirmar cadastro.

### Resultado Esperado

* Cadastro rejeitado.
* Mensagem informando que o e-mail já está em uso.

### Status

Não Executado

---

## CT-FUNC-003 - Login com Credenciais Válidas

### Requisito

REQ-002 - Autenticação de Usuário

### Tipo

Funcional

### Prioridade

Alta

### Pré-condições

* Usuário previamente cadastrado.

### Passos

1. Acessar tela de login.
2. Informar e-mail válido.
3. Informar senha válida.
4. Confirmar autenticação.

### Resultado Esperado

* Login realizado com sucesso.
* Usuário direcionado para a área principal.

### Status

Não Executado

---

## CT-FUNC-004 - Login com Senha Inválida

### Requisito

REQ-002 - Autenticação de Usuário

### Tipo

Funcional

### Prioridade

Alta

### Pré-condições

* Usuário cadastrado.

### Passos

1. Acessar tela de login.
2. Informar e-mail válido.
3. Informar senha incorreta.
4. Confirmar autenticação.

### Resultado Esperado

* Login rejeitado.
* Mensagem de erro exibida ao usuário.

### Status

Não Executado

---

# Casos de Teste de Integração

## CT-INT-001 - Integração entre Frontend e API de Login

### Requisito

REQ-002 - Autenticação de Usuário

### Tipo

Integração

### Prioridade

Alta

### Pré-condições

* API disponível.
* Usuário cadastrado.

### Passos

1. Realizar login através da interface.
2. Enviar requisição para API.
3. Receber resposta da autenticação.

### Resultado Esperado

* API retorna autenticação válida.
* Interface recebe e processa a resposta corretamente.

### Status

Não Executado

---

# Casos de Teste E2E

## CT-E2E-001 - Fluxo Completo de Cadastro e Login

### Requisito

REQ-001
REQ-002

### Tipo

E2E

### Prioridade

Alta

### Pré-condições

* Usuário não cadastrado.

### Passos

1. Realizar cadastro.
2. Confirmar cadastro.
3. Efetuar login.
4. Acessar área principal.

### Resultado Esperado

* Fluxo executado sem erros.
* Usuário autenticado ao final do processo.

### Status

Não Executado

---

# Casos de Teste Não Funcionais

## CT-SEG-001 - Armazenamento Seguro de Senhas

### Requisito

RNF-001 - Segurança de Autenticação

### Tipo

Segurança

### Prioridade

Alta

### Pré-condições

* Usuário cadastrado.

### Passos

1. Criar usuário.
2. Consultar registro armazenado.
3. Verificar armazenamento da senha.

### Resultado Esperado

* Senha não armazenada em texto puro.
* Senha protegida por algoritmo de hash.

### Status

Não Executado

---

## CT-PERF-001 - Tempo de Resposta da Autenticação

### Requisito

RNF-002 - Tempo de Resposta

### Tipo

Desempenho

### Prioridade

Média

### Pré-condições

* Ambiente operacional disponível.

### Passos

1. Realizar autenticação.
2. Medir tempo de resposta.

### Resultado Esperado

* Tempo de resposta inferior ao limite definido pelo requisito.

### Status

Não Executado

---

# Controle de Execução

## Status Possíveis

| Status        | Descrição                       |
| ------------- | ------------------------------- |
| Não Executado | Teste ainda não realizado       |
| Em Execução   | Teste em andamento              |
| Aprovado      | Resultado conforme esperado     |
| Reprovado     | Resultado diferente do esperado |
| Bloqueado     | Impedimento para execução       |

---

# Rastreabilidade

Todos os casos de teste deverão possuir vínculo com os requisitos do sistema.

Exemplo:

| Caso de Teste | Requisito        |
| ------------- | ---------------- |
| CT-FUNC-001   | REQ-001          |
| CT-FUNC-002   | REQ-001          |
| CT-FUNC-003   | REQ-002          |
| CT-FUNC-004   | REQ-002          |
| CT-INT-001    | REQ-002          |
| CT-E2E-001    | REQ-001, REQ-002 |
| CT-SEG-001    | RNF-001          |
| CT-PERF-001   | RNF-002          |

---

# Histórico de Alterações

| Data       | Versão | Descrição                    |
| ---------- | ------ | ---------------------------- |
| 04/06/2026 | 1.0    | Criação inicial do documento |

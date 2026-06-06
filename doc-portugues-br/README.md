# 📚 doc-msp.br-framework

> Um **manual vivo de engenharia de software** baseado no **MPS.BR / MR-MPS-SW** (níveis G a A). Cada pasta é **autossuficiente**: você entende propósito, conteúdo e evolução de cada área sem navegar por outras pastas.

Serve como **guia de estudo**, **modelo para empresas** e **referência profissional** de maturidade de processos.

## 🧭 Organização
Por **área de processo** (disciplina); dentro de cada área, a documentação **evolui por nível MPS.BR**. Os níveis não duplicam a estrutura — só definem maturidade, critérios e capacidades.

```
doc-portugues-br/
├── README.md
├── niveis-mps/        ← definição de cada nível (G a A)
├── areas-processo/    ← as 14 disciplinas, cada uma autossuficiente
│   └── <área>/  README.md + nivel-X.md
├── artefatos/         ← 1 exemplo real de cada arquivo
├── templates-base/    ← templates genéricos
└── exemplos/          ← projetos de referência por maturidade
```

## 🎚️ Níveis MPS.BR

| Nível | Nome | Foco |
|---|---|---|
| [Nível G](niveis-mps/nivel-G.md) | Parcialmente Gerenciado | Requisitos e projeto |
| [Nível F](niveis-mps/nivel-F.md) | Gerenciado | Configuração, medição e qualidade |
| [Nível E](niveis-mps/nivel-E.md) | Parcialmente Definido | Processo e arquitetura |
| [Nível D](niveis-mps/nivel-D.md) | Largamente Definido | Organização e processos |
| [Nível C](niveis-mps/nivel-C.md) | Definido | Decisões, riscos e reutilização |
| [Nível B](niveis-mps/nivel-B.md) | Gerenciado Quantitativamente | Controle estatístico |
| [Nível A](niveis-mps/nivel-A.md) | Em Otimização | Melhoria contínua |

## 🗂️ Áreas de processo

| Área | Disciplina | Disponível |
|---|---|---|
| 📋 [`requisitos`](areas-processo/requisitos/README.md) | Requisitos | a partir do nível G |
| 📅 [`projetos`](areas-processo/projetos/README.md) | Projetos | a partir do nível G |
| 🗂️ [`configuracao`](areas-processo/configuracao/README.md) | Configuração | a partir do nível F |
| 📊 [`medicao`](areas-processo/medicao/README.md) | Medição | a partir do nível F |
| ✅ [`qualidade`](areas-processo/qualidade/README.md) | Qualidade | a partir do nível F |
| 🏗️ [`arquitetura`](areas-processo/arquitetura/README.md) | Arquitetura | a partir do nível F |
| 🔗 [`integracao`](areas-processo/integracao/README.md) | Integração | a partir do nível E |
| 🏛️ [`organizacao`](areas-processo/organizacao/README.md) | Organização | a partir do nível D |
| ⚙️ [`processos`](areas-processo/processos/README.md) | Processos | a partir do nível D |
| 🧭 [`decisoes`](areas-processo/decisoes/README.md) | Decisões | a partir do nível C |
| ♻️ [`reutilizacao`](areas-processo/reutilizacao/README.md) | Reutilização | a partir do nível C |
| ⚠️ [`riscos`](areas-processo/riscos/README.md) | Riscos | a partir do nível C |
| 📈 [`gerencia-quantitativa`](areas-processo/gerencia-quantitativa/README.md) | Gerência Quantitativa | a partir do nível B |
| 🚀 [`melhoria-continua`](areas-processo/melhoria-continua/README.md) | Melhoria Contínua | a partir do nível A |

## 🚦 Por onde começar
1. Leia os [níveis MPS.BR](niveis-mps/nivel-G.md).
2. Escolha uma [área](areas-processo/requisitos/README.md) e leia o README.
3. Siga a evolução `nivel-G → nivel-A` dentro da área.
4. Use os [templates-base](templates-base/requisito.md) e veja [exemplos reais](artefatos/README.md).

## 🧱 Princípios
- **Autossuficiência** · **Zero duplicação** · **Por disciplina** · **Níveis como evolução** · **Self-contained**.

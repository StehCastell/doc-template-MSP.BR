# 🗂️ Área de Processo — Configuração

> Esta pasta é **autossuficiente**: tudo o que você precisa para entender a área está aqui.

## 📌 O que é esta área no MPS.BR
Controle de versões, baselines e mudanças nos artefatos. Corresponde à **Gerência de Configuração (GCO)**.

## 🎯 Qual problema ela resolve
Resolve o **'qual versão é a verdadeira?'** e a perda de histórico.

## ✅ O que entra nesta área
- Controle de versões
- Linha-base (baseline)
- Plano de gerência de configuração
- Itens de configuração

## 🚫 O que NÃO entra nesta área
- Mudança de requisitos (→ requisitos)
- Decisões de design (→ arquitetura)

## 📈 Como evolui do nível G ao A

| Nível MPS.BR | Evolução da área |
|---|---|
| Nível G — Parcialmente Gerenciado | — (ainda não aplicável) |
| Nível F — Gerenciado | Versões e baselines controladas. |
| Nível E — Parcialmente Definido | Política de configuração padronizada. |
| Nível D — Largamente Definido | Configuração integrada ao processo. |
| Nível C — Definido | Inclui controle de decisões/reutilização. |
| Nível B — Gerenciado Quantitativamente | Integridade medida. |
| Nível A — Em Otimização | Processo otimizado e automatizado. |

## 🗂️ Arquivos desta área (evolução por nível)
- [`nivel-F.md`](nivel-F.md) — capacidade: Versões e baselines controladas.
- [`nivel-E.md`](nivel-E.md) — capacidade: Política de configuração padronizada.
- [`nivel-D.md`](nivel-D.md) — capacidade: Configuração integrada ao processo.
- [`nivel-C.md`](nivel-C.md) — capacidade: Inclui controle de decisões/reutilização.
- [`nivel-B.md`](nivel-B.md) — capacidade: Integridade medida.
- [`nivel-A.md`](nivel-A.md) — capacidade: Processo otimizado e automatizado.

## 💡 Exemplos de uso
- Definir estratégia de branches.
- Congelar baseline antes da release.

## 🔗 Relação com outras áreas
- **projetos** — releases dependem de baselines.
- **qualidade** — auditoria verifica integridade.

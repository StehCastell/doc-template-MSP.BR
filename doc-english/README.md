# 📚 doc-msp.br-framework

> A **living software-engineering handbook** based on **MPS.BR / MR-MPS-SW** (levels G to A). Each folder is **self-contained**: you understand the purpose, content and evolution of every area without navigating elsewhere.

Serves as a **study guide**, a **company model** and a **professional reference** for process maturity.

## 🧭 Organization
By **process area** (discipline); within each area, documentation **evolves by MPS.BR level**. Levels do not duplicate the structure — they only define maturity, criteria and capabilities.

```
doc-english/
├── README.md
├── mps-levels/        ← definition of each level (G to A)
├── process-areas/     ← the 14 disciplines, each self-contained
│   └── <area>/  README.md + level-X.md
├── artifacts/         ← one real example of each file
├── base-templates/    ← generic templates
└── examples/          ← reference projects by maturity
```

## 🎚️ MPS.BR Levels

| Level | Name | Focus |
|---|---|---|
| [Level G](mps-levels/level-G.md) | Partially Managed | Requirements and project |
| [Level F](mps-levels/level-F.md) | Managed | Configuration, measurement and quality |
| [Level E](mps-levels/level-E.md) | Partially Defined | Process and architecture |
| [Level D](mps-levels/level-D.md) | Largely Defined | Organization and processes |
| [Level C](mps-levels/level-C.md) | Defined | Decisions, risks and reuse |
| [Level B](mps-levels/level-B.md) | Quantitatively Managed | Statistical control |
| [Level A](mps-levels/level-A.md) | Optimizing | Continuous improvement |

## 🗂️ Process areas

| Area | Discipline | Available |
|---|---|---|
| 📋 [`requirements`](process-areas/requirements/README.md) | Requirements | from level G |
| 📅 [`projects`](process-areas/projects/README.md) | Projects | from level G |
| 🗂️ [`configuration`](process-areas/configuration/README.md) | Configuration | from level F |
| 📊 [`measurement`](process-areas/measurement/README.md) | Measurement | from level F |
| ✅ [`quality`](process-areas/quality/README.md) | Quality | from level F |
| 🏗️ [`architecture`](process-areas/architecture/README.md) | Architecture | from level F |
| 🔗 [`integration`](process-areas/integration/README.md) | Integration | from level E |
| 🏛️ [`organization`](process-areas/organization/README.md) | Organization | from level D |
| ⚙️ [`processes`](process-areas/processes/README.md) | Processes | from level D |
| 🧭 [`decisions`](process-areas/decisions/README.md) | Decisions | from level C |
| ♻️ [`reuse`](process-areas/reuse/README.md) | Reuse | from level C |
| ⚠️ [`risk-management`](process-areas/risk-management/README.md) | Risk Management | from level C |
| 📈 [`quantitative-management`](process-areas/quantitative-management/README.md) | Quantitative Management | from level B |
| 🚀 [`continuous-improvement`](process-areas/continuous-improvement/README.md) | Continuous Improvement | from level A |

## 🚦 Where to start
1. Read the [MPS.BR levels](mps-levels/level-G.md).
2. Pick an [area](process-areas/requirements/README.md) and read the README.
3. Follow the evolution `level-G → level-A` within the area.
4. Use the [base-templates](base-templates/requirement.md) and see [real examples](artifacts/README.md).

## 🧱 Principles
- **Self-sufficiency** · **Zero duplication** · **By discipline** · **Levels as evolution** · **Self-contained**.

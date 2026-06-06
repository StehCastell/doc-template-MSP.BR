# 🗂️ Process Area — Configuration

> This folder is **self-contained**: everything you need to understand the area is here.

## 📌 What this area is in MPS.BR
Version, baseline and change control over artifacts. Maps to **Configuration Management (GCO)**.

## 🎯 What problem it solves
Solves **'which version is real?'** and loss of history.

## ✅ What belongs in this area
- Version control
- Baseline
- Configuration management plan
- Configuration items

## 🚫 What does NOT belong in this area
- Requirements change (→ requirements)
- Design decisions (→ architecture)

## 📈 How it evolves from level G to A

| Level MPS.BR | Evolution of the area |
|---|---|
| Level G — Partially Managed | — (not applicable yet) |
| Level F — Managed | Controlled versions and baselines. |
| Level E — Partially Defined | Standardized configuration policy. |
| Level D — Largely Defined | Configuration integrated into the process. |
| Level C — Defined | Includes control of decisions/reuse. |
| Level B — Quantitatively Managed | Integrity measured. |
| Level A — Optimizing | Optimized and automated process. |

## 🗂️ Files in this area (evolution by level)
- [`level-F.md`](level-F.md) — capability: Controlled versions and baselines.
- [`level-E.md`](level-E.md) — capability: Standardized configuration policy.
- [`level-D.md`](level-D.md) — capability: Configuration integrated into the process.
- [`level-C.md`](level-C.md) — capability: Includes control of decisions/reuse.
- [`level-B.md`](level-B.md) — capability: Integrity measured.
- [`level-A.md`](level-A.md) — capability: Optimized and automated process.

## 💡 Usage examples
- Define a branching strategy.
- Freeze a baseline before release.

## 🔗 Relationship with other areas
- **projects** — releases depend on baselines.
- **quality** — audits verify integrity.

# 🏗️ Process Area — Architecture

> This folder is **self-contained**: everything you need to understand the area is here.

## 📌 What this area is in MPS.BR
Technical structure of the solution: components, layers and decisions. Supports **Product Design and Construction**.

## 🎯 What problem it solves
Solves **implicit, inconsistent technical decisions**.

## ✅ What belongs in this area
- Architecture overview
- Architecture by layer/platform
- Architectural decisions (ADR)
- Technical constraints

## 🚫 What does NOT belong in this area
- What the system does (→ requirements)
- Planning (→ projects)

## 📈 How it evolves from level G to A

| Level MPS.BR | Evolution of the area |
|---|---|
| Level G — Partially Managed | — (not applicable yet) |
| Level F — Managed | Documented architecture (optional). |
| Level E — Partially Defined | Defined project architecture. |
| Level D — Largely Defined | Organizational architectural patterns. |
| Level C — Defined | Architecture linked to decisions/reuse. |
| Level B — Quantitatively Managed | Architectural attributes measured. |
| Level A — Optimizing | Architecture evolves via innovation. |

## 🗂️ Files in this area (evolution by level)
- [`level-F.md`](level-F.md) — capability: Documented architecture (optional).
- [`level-E.md`](level-E.md) — capability: Defined project architecture.
- [`level-D.md`](level-D.md) — capability: Organizational architectural patterns.
- [`level-C.md`](level-C.md) — capability: Architecture linked to decisions/reuse.
- [`level-B.md`](level-B.md) — capability: Architectural attributes measured.
- [`level-A.md`](level-A.md) — capability: Architecture evolves via innovation.

## 💡 Usage examples
- Document the backend/frontend API contract.
- Record a technology-choice ADR.

## 🔗 Relationship with other areas
- **requirements** — realizes non-functional requirements.
- **integration** — defines how to integrate.
- **processes** — implements the architecture.

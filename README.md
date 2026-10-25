Zero-Division Containers
Author: Joanmer Ramos (Joy)
Current version: v0.1
Date of initial draft: October 24, 2026
Status: Draft — work in progress; not a complete or verified mathematical theory.

Overview
This repository documents an exploratory arithmetic system in which division of an integer by zero is defined to create a new object called a container, written n|0. The container stores the integer value n together with a zero divisor.

The project distinguishes ordinary integer values from container objects and explores operations that either preserve a container or extract its value.

Provisional rules at a glance
n/0 creates a new container with value n.
Each creation has its own identity, even when two containers hold the same value.
Preserving addition: n|0 ⊕ m = (n+m)|0.
Extracting addition: (n|0) + m = n+m.
Extraction: E(n|0) = n.
Proposed zero-multiplication rule: n × 0 = n|0.
Dividing an extracted integer by zero creates a new container.
These are proposed rules for this system, not claims about conventional arithmetic.

Repository contents
Zero-Division-Containers-v0.1.md — the draft, including examples, open questions, and the author's note.
Zero-Division-Containers-v0.1.pdf — a PDF reading copy of the same draft.
Open questions
The draft identifies questions about container identity, equality of values versus equality of objects, the distinct roles of ⊕ and +, commutativity, multiplication and division involving containers, and evaluation order in mixed expressions.

Scope and status
This repository records an early proposal. The rules have not yet been fully formalized, checked for mutual consistency, or proved to satisfy the listed properties. Future revisions should document changes explicitly.

Date note
Licencia y Citación
Este trabajo está protegido bajo la licencia Creative Commons Atribución 4.0 Internacional (CC BY 4.0).

Para citar este trabajo: Ramos Vera, J. J. (2026). Theory of Zero-Division Containers: Mathematical Framework and Arithmetic Implementation (v0.1). Zenodo. https://doi.org

The first draft was prepared on October 24, 2026, a date the author regards as a personal Pythagorean milestone.

Citation
Ramos, J. (2026). Zero-Division Containers: Draft of an Arithmetic System (v0.1, draft).
# zero-division-containers
This formal preprint introduces the baseline architecture of the Theory of Zero-Division Containers, presenting a novel conceptual approach to handling division-by-zero operations within bounded arithmetic systems. This repository aggregates the foundational paper (PDF), the raw markdown specifications (.md), and the architectural documentation.
## Licencia y Citación

Este trabajo está protegido bajo la licencia **Creative Commons Atribución 4.0 Internacional (CC BY 4.0)**. 

Para citar este trabajo:
Ramos Vera, J. J. (2026). *Theory of Zero-Division Containers: Mathematical Framework and Arithmetic Implementation (v0.1)*. Zenodo. https://doi.org

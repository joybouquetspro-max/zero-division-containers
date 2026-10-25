# Zero-Division Containers: Draft of an Arithmetic System

**Author:** Joanmer Ramos (Joy)  
**Date:** October 24, 2026  
**Version:** v0.1  
**Status:** Draft, work in progress. This is not a complete or verified theory.

## Abstract

This draft proposes an arithmetic system in which dividing an integer by zero is a defined operation. The result is not an ordinary number but a new object, the *container* `n|0`, which stores the value `n` together with a zero divisor. The draft presents the objects, the provisional rules, worked examples, and the decisions that are still open.

## Motivation

The motivation is to give meaning to dividing an integer by zero without the integer disappearing: the result keeps the original value inside a new object.

## Objects

- **Ordinary integers:** `n`, with their usual arithmetic.
- **Containers:** `n|0`, made of an integer value `n` and a zero divisor. Each container has its own identity: they are written `C₁`, `C₂`, etc. when they need to be told apart.

## Provisional rules

1. **Creation.** `n/0` creates a new container with value `n`.
2. **Identity.** Every time a container is created, it is distinct from all previous ones even if it has the same value: `C₁ ≠ C₂` even if both hold 13.
3. **Preserving addition (⊕).** `n|0 ⊕ m = (n+m)|0`. The container remains.
4. **Extracting addition (+).** `(n|0) + m = n + m`. The container disappears and an integer remains.
5. **Extraction.** `E(n|0) = n`.
6. **Multiplication by zero.** `n × 0 = n|0`. Multiplying by zero does not make `n` disappear: it stores it in a container.
7. **Reappearance.** Dividing by zero an integer obtained by extraction creates a new container (rules 1 and 2).

## Worked examples

**Example 1.** `10|0 ⊕ 3 = 13|0`. The container is preserved.

**Example 2.** `(13|0) + 2 = 15`. Adding with an integer extracts the value.

**Example 3, container cycle.** Let `C₁ = 13|0`. Then `E(C₁) = 13`. Next, `13/0 = C₂ = 13|0`, with `C₁ ≠ C₂`. As long as no integer is added with `+`, the container stays.

**Example 4.** `10 × 0 = 10|0`. Multiplying by zero keeps the 10 inside a container, just like `10/0 = 10|0`.

## Properties to prove

- `E(x ⊕ y) = E(x) + E(y)`.
- `E(n/0) = n`.
- Commutativity and associativity of `⊕`.
- Consistency of evaluation order in mixed expressions.

## Open questions

1. **Container identity.** If `C₁ ≠ C₂` with the same value, we need a formal definition of what tells them apart (for example, a label or a creation counter).
2. **Two equalities.** Equality of value should be separated from equality of structure, with different symbols.
3. **Use of ⊕ and +.** State without ambiguity when each one applies.
4. **Commutativity.** Do `(13|0) + 2` and `2 + (13|0)` give the same result?
5. **Multiplication and division of containers.** What is `(n|0)/0`, and what happens with `(n|0) × m`?
6. **Mixed expressions.** What is `(n|0) × 0`, and in what order are expressions like `12 + 2/0 × 0` evaluated?

## Author's note — October 24, 2026

This first draft was written on October 24, 2026, a date that holds personal significance for the author as a Pythagorean milestone. The author marks this day as a meaningful point in her mathematical journey: the beginning of a system she intends to explore, refine, and develop over time.

This document records the ideas and provisional rules established on this date. It is a work in progress, not a verified mathematical theory.

## Next steps

1. Formalize the rules with explicit definitions and axioms.
2. Resolve the open questions.
3. Prove or refute the listed properties.

## How to cite

Ramos, J. (2026). *Zero-Division Containers: Draft of an Arithmetic System* (v0.1, draft).

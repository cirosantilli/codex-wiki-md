# Golden ratio approximation for MAX-2SAT

↑ **Parent:** [Maximum 2-satisfiability](maximum-2-satisfiability.md)

When each variable appears in at most one normalized singleton [clause](clause-of-a-boolean-formula.md), satisfy that favored [literal](boolean-literal.md) with [probability](probability.md) $p>1/2$ and choose independent variables. Every proper binary [clause](clause-of-a-boolean-formula.md) is then satisfied with [probability](probability.md) at least $1-p^2$, and every singleton with [probability](probability.md) $p$. Maximize the common lower bound by $p=1-p^2$, giving the reciprocal of the [golden ratio](golden-ratio.md). The [method of conditional probabilities](method-of-conditional-probabilities.md) derandomizes the construction, obtaining [approximation ratio](approximation-ratio.md) $p$. Tautologies are harmless; the singleton restriction must be applied after removing repeated [literals](boolean-literal.md) within [clauses](clause-of-a-boolean-formula.md).

## ↑ Ancestors (10)

1. [Maximum 2-satisfiability](maximum-2-satisfiability.md)
2. [Boolean satisfiability problem](boolean-satisfiability-problem.md)
3. [NP-completeness](np-completeness.md)
4. [NP-hardness](np-hardness.md)
5. [Polynomial-time many-one reduction](polynomial-time-many-one-reduction.md)
6. [Polynomial-time reduction](polynomial-time-reduction.md)
7. [Computational complexity theory](computational-complexity-theory.md)
8. [Theoretical computer science](theoretical-computer-science.md)
9. [Computer science](computer-science-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-37/6/d/solution.md)

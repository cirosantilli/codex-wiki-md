# Exactly-one constraint

↑ **Parent:** [Boolean satisfiability problem](boolean-satisfiability-problem.md)

A restriction requiring exactly one member of a [set](set-split.md) of [Boolean variables](boolean-variable.md) to be true. A direct [conjunctive normal form](conjunctive-normal-form.md) encoding combines one at-least-one [Boolean clause](clause-of-a-boolean-formula.md), $p_1\lor\cdots\lor p_q$, with $\binom q2$ at-most-one [Boolean clauses](clause-of-a-boolean-formula.md), $\neg p_i\lor\neg p_j$ for $i<j$. The first supplies existence and the second supplies uniqueness. For $q=0$, the empty at-least-one [Boolean clause](clause-of-a-boolean-formula.md) correctly makes the condition unsatisfiable.

## ↑ Ancestors (9)

1. [Boolean satisfiability problem](boolean-satisfiability-problem.md)
2. [NP-completeness](np-completeness.md)
3. [NP-hardness](np-hardness.md)
4. [Polynomial-time many-one reduction](polynomial-time-many-one-reduction.md)
5. [Polynomial-time reduction](polynomial-time-reduction.md)
6. [Computational complexity theory](computational-complexity-theory.md)
7. [Theoretical computer science](theoretical-computer-science-split.md)
8. [Computer science](computer-science-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Direct SAT encoding of finite-domain constraints](direct-sat-encoding-of-finite-domain-constraints.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence/2/e/solution.md)

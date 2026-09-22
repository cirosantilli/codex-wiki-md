# Unit propagation

↑ **Parent:** [SAT solver](sat-solver.md)

If all but one [literal](boolean-literal.md) of a [Boolean clause](clause-of-a-boolean-formula.md) are false under a partial [Boolean valuation](boolean-valuation.md), the remaining [literal](boolean-literal.md) must be true in any extension satisfying the clause. Repeatedly make such forced assignments, remove satisfied [Boolean clauses](clause-of-a-boolean-formula.md) and remove false [literals](boolean-literal.md) from the others. An empty [Boolean clause](clause-of-a-boolean-formula.md) proves that the current partial [Boolean valuation](boolean-valuation.md) has no satisfying extension. This is sound because every step is forced by an original or already implied [Boolean clause](clause-of-a-boolean-formula.md); it is not by itself a complete [SAT](boolean-satisfiability-problem.md) decision procedure.

## ↑ Ancestors (10)

1. [SAT solver](sat-solver.md)
2. [Boolean satisfiability problem](boolean-satisfiability-problem.md)
3. [NP-completeness](np-completeness.md)
4. [NP-hardness](np-hardness.md)
5. [Polynomial-time many-one reduction](polynomial-time-many-one-reduction.md)
6. [Polynomial-time reduction](polynomial-time-reduction.md)
7. [Computational complexity theory](computational-complexity-theory.md)
8. [Theoretical computer science](theoretical-computer-science-split.md)
9. [Computer science](computer-science-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Direct SAT encoding of finite-domain constraints](direct-sat-encoding-of-finite-domain-constraints.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence/2/f/solution.md)
- [SAT solver](sat-solver.md)

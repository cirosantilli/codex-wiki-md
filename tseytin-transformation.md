# Tseytin transformation

↑ **Parent:** [Conjunctive normal form](conjunctive-normal-form.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tseytin_transformation)

Introduce a [Boolean variable](boolean-variable.md) for each gate output and impose its equivalence to the gate's input function with a constant number of [clauses](clause-of-a-boolean-formula.md). A final unit [clause](clause-of-a-boolean-formula.md) forces acceptance. For a bounded-fan-in [Boolean circuit](boolean-circuit.md), the formula size is linear in the gate count and it is satisfiable exactly when some input makes the [Boolean circuit](boolean-circuit.md) output one. Auxiliary variables extend the satisfying assignments; this is equisatisfiability, not equality as functions of the enlarged variable set.

## ↑ Ancestors (11)

1. [Conjunctive normal form](conjunctive-normal-form.md)
2. [Boolean formula](boolean-formula.md)
3. [Boolean satisfiability problem](boolean-satisfiability-problem.md)
4. [NP-completeness](np-completeness.md)
5. [NP-hardness](np-hardness.md)
6. [Polynomial-time many-one reduction](polynomial-time-many-one-reduction.md)
7. [Polynomial-time reduction](polynomial-time-reduction.md)
8. [Computational complexity theory](computational-complexity-theory.md)
9. [Theoretical computer science](theoretical-computer-science.md)
10. [Computer science](computer-science-split.md)
11. [Codex Wiki](split.md)

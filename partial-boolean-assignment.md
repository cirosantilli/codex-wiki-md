# Partial Boolean assignment

↑ **Parent:** [Boolean satisfiability problem](boolean-satisfiability-problem.md)

A [partial Boolean assignment](partial-boolean-assignment.md) gives [truth values](truth-value.md) to some of a [Boolean formula](boolean-formula.md)'s [Boolean variables](boolean-variable.md). An extension is a complete [Boolean valuation](boolean-valuation.md) agreeing on the assigned [Boolean variables](boolean-variable.md). In [CNF](conjunctive-normal-form.md), a [Boolean clause](clause-of-a-boolean-formula.md) containing a true assigned [Boolean literal](boolean-literal.md) is already satisfied; a [Boolean clause](clause-of-a-boolean-formula.md) whose every [Boolean literal](boolean-literal.md) is assigned false rules out all extensions. A [Boolean clause](clause-of-a-boolean-formula.md) with no true assigned [Boolean literal](boolean-literal.md) and at least one unassigned [Boolean variable](boolean-variable.md) is unresolved. An unresolved [Boolean clause](clause-of-a-boolean-formula.md) need not have a compatible extension with the other [Boolean clauses](clause-of-a-boolean-formula.md).

For $F$ in [Boolean satisfiability problem](boolean-satisfiability-problem.md), setting $x=y=0$ already falsifies $C_1$, so both choices of $z$ can be discarded. Setting only $x=0$ leaves $C_1$ unresolved and forces $y=1$ if a [satisfying assignment](satisfying-assignment.md) is to survive; then $C_3$ forces $z=0$. Branching on an unassigned [Boolean variable](boolean-variable.md) into its two [truth values](truth-value.md) and discarding branches with a false [Boolean clause](clause-of-a-boolean-formula.md) is sound: every [satisfying assignment](satisfying-assignment.md) follows one branch and cannot extend a false [Boolean clause](clause-of-a-boolean-formula.md). If all branches are eliminated, the original [Boolean formula](boolean-formula.md) is an [unsatisfiable Boolean formula](unsatisfiable-boolean-formula.md).

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

## ← Incoming links (1)

- [Partial Boolean assignment](partial-boolean-assignment.md)

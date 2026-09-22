# Verifying a satisfying assignment

↑ **Parent:** [Satisfying assignment](satisfying-assignment.md)

For a [CNF](conjunctive-normal-form.md) input with $n$ [Boolean variables](boolean-variable.md), $m$ [Boolean clauses](clause-of-a-boolean-formula.md), and $L$ [Boolean literal](boolean-literal.md) occurrences, first check that the supplied [Boolean valuation](boolean-valuation.md) gives each input [Boolean variable](boolean-variable.md) exactly one [truth value](truth-value.md). Evaluate each [Boolean literal](boolean-literal.md) by lookup or [logical negation](negation.md), each [Boolean clause](clause-of-a-boolean-formula.md) by [logical disjunction](logical-disjunction.md), and the [Boolean formula](boolean-formula.md) by [logical conjunction](logical-conjunction.md). Indexed [Boolean variables](boolean-variable.md) and constant-cost lookups give an $O(n+m+L)$ operation count; with a finite [binary string](binary-string.md) encoding the check still takes [polynomial time](polynomial-time.md). Thus a [satisfying assignment](satisfying-assignment.md) is a [certificate in computational complexity](certificate-complexity.md) for [SAT](boolean-satisfiability-problem.md), proving that [SAT](boolean-satisfiability-problem.md) belongs to [NP](np-complexity.md). Finding it by exhaustive checking can require $2^n$ candidate [Boolean valuations](boolean-valuation.md); this enumeration cost is not a lower bound on every possible [SAT](boolean-satisfiability-problem.md) [algorithm](algorithm-split.md).[CS 252, Lecture 8: Constraint Satisfaction Problems, p. 3, §3 opening paragraph: assignments as certificates and membership in NP](cs-252-lecture-8-constraint-satisfaction-problems-carnegie-mellon-university.md)

## ↑ Ancestors (10)

1. [Satisfying assignment](satisfying-assignment.md)
2. [Boolean satisfiability problem](boolean-satisfiability-problem.md)
3. [NP-completeness](np-completeness.md)
4. [NP-hardness](np-hardness.md)
5. [Polynomial-time many-one reduction](polynomial-time-many-one-reduction.md)
6. [Polynomial-time reduction](polynomial-time-reduction.md)
7. [Computational complexity theory](computational-complexity-theory.md)
8. [Theoretical computer science](theoretical-computer-science-split.md)
9. [Computer science](computer-science-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Boolean satisfiability problem](boolean-satisfiability-problem.md)

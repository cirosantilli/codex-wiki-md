# Literal-frequency greedy approximation for MAX-SAT

↑ **Parent:** [Maximum satisfiability](maximum-satisfiability.md)

In the residual unsatisfied formula, choose a [Boolean literal](boolean-literal.md) contained in the largest number $a$ of clauses and make it true. Its opposite occurs in at most $a$ clauses, since it too was an eligible literal. The step permanently satisfies $a$ clauses; only clauses containing the opposite can become empty, so it loses at most $a$ clauses. Delete satisfied clauses and false literals and repeat. No satisfied clause or newly empty clause is counted twice. Summing gives total lost nonempty clauses at most total satisfied clauses $G$. All initially nonempty clauses are eventually in one of these classes, so $G\geq N_+/2\geq\operatorname{OPT}/2$. Initial empty clauses can never be satisfied and are excluded from $N_+$. This proves the [approximation algorithm](approximation-algorithm.md) guarantee even with tautological clauses or repeated literals.

## ↑ Ancestors (10)

1. [Maximum satisfiability](maximum-satisfiability.md)
2. [Boolean satisfiability problem](boolean-satisfiability-problem.md)
3. [NP-completeness](np-completeness.md)
4. [NP-hardness](np-hardness.md)
5. [Polynomial-time many-one reduction](polynomial-time-many-one-reduction.md)
6. [Polynomial-time reduction](polynomial-time-reduction.md)
7. [Computational complexity theory](computational-complexity-theory.md)
8. [Theoretical computer science](theoretical-computer-science.md)
9. [Computer science](computer-science-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Maximum satisfiability](maximum-satisfiability.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-35/4/solution.md)

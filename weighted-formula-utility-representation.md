# Weighted formula utility representation

↑ **Parent:** [Utility function](utility-function-split.md)

A finite rule base pairs [propositional formulas](propositional-formula.md) with weights and sums the weights of the formulas satisfied by a [Boolean valuation](boolean-valuation.md). Over a finite set $S$, associate one [Boolean variable](boolean-variable.md) to membership of each element. Any [utility function](utility-function-split.md) $u:2^S\to\mathbb R$ is represented by giving each subset's [minterm](minterm.md) weight $u(T)$. Exactly one rule fires at each valuation, so at most $2^{|S|}$ rules suffice. This bound counts rules, not the symbols required to write all formulas.

For computational questions, the weight encoding matters. Binary [rational numbers](rational-number.md) permit exact addition and comparison in [polynomial time](polynomial-time.md); unrestricted real constants do not specify an ordinary finite input encoding.

## ↑ Ancestors (6)

1. [Utility function](utility-function-split.md)
2. [Mathematical finance](mathematical-finance-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Equivalence of weighted formula utility representations](equivalence-of-weighted-formula-utility-representations.md)
- [Finite-variable dependence of a propositional rule base](finite-variable-dependence-of-a-propositional-rule-base.md)
- [Solution](past-exam-of-the-msc-in-advanced-computer-science-course-of-the-university-of-oxford/2023/computational-game-theory/1/c/solution.md)

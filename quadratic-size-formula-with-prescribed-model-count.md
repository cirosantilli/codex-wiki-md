# Quadratic-size formula with prescribed model count

↑ **Parent:** [Satisfying assignment](satisfying-assignment.md)

For each $0\leq k\leq2^n$, a [propositional formula](propositional-formula.md) over $n$ specified variables can have exactly $k$ [satisfying assignments](satisfying-assignment.md) and length $O(n^2)$. For $0<k<2^n$, interpret a [Boolean valuation](boolean-valuation.md) as the [binary number](binary-number.md) $x_1\cdots x_n$ and test whether it is less than $k=b_1\cdots b_n$.

For every position $i$ with $b_i=1$, use a conjunction asserting that all earlier [bits](bit.md) equal $b_j$ and $x_i=0$, leaving later [bits](bit.md) unrestricted. Take the disjunction of these terms. Each satisfying assignment has a unique first differing position, so the terms are disjoint, and their counts sum to $\sum_{i:b_i=1}2^{n-i}=k$. Their combined length is $O(1+2+\cdots+n)=O(n^2)$. Use [logical falsity](logical-falsity.md) and [logical truth](logical-truth.md) at the two endpoints. The count is over all $n$ variables, including those absent from an individual term or from the whole formula.

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

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/digital-systems-linear-algebra-and-introduction-to-formal-proof/7/d/solution.md)

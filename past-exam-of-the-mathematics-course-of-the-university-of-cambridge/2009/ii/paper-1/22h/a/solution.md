<h1 id="22h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Baire category theorem](../../../../../../baire-category-theorem.md) states that a complete [metric space](../../../../../../metric-space.md) is a [Baire space](../../../../../../baire-space.md): the intersection of countably many open dense sets is dense. Equivalently, a nonempty open subset cannot be a countable union of nowhere dense sets.

Let $U_n$ be open dense and $O$ any nonempty open set. Choose a closed ball $B_1$ of positive radius at most $1/2$ inside $O\cap U_1$. Inductively choose $B_{n+1}$ inside the interior of $B_n$ intersected with $U_{n+1}$, with positive radius at most $2^{-(n+1)}$. Density makes this intersection nonempty, and openness supplies a sufficiently small closed ball. The centres form a [Cauchy sequence](../../../../../../cauchy-sequence.md) because all later centres lie in $B_n$, whose diameter tends to zero. Completeness gives a limit $x$. Since each ball is closed and contains all later centres, $x\in B_n$ for every $n$. Thus $x\in O\cap\bigcap_n U_n$, proving density. Applying this to complements of the closures of nowhere dense sets gives the equivalent formulation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [22H](../../22h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

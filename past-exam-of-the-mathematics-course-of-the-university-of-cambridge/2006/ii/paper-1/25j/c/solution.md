<h1 id="25j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The first event is a [tail event](../../../../../../tail-event.md): for any $m$ it equals $\bigcup_{N\geq m}\bigcap_{n\geq N}\{X_n\leq0\}$, measurable in $\sigma(X_m,X_{m+1},\ldots)$.

Convergence of the partial sums is also a [tail event](../../../../../../tail-event.md). For any $m$, subtracting the finite real sum $X_1+\cdots+X_{m-1}$ shows that convergence is equivalent to convergence of $\sum_{j=m}^nX_j$. The Cauchy criterion expresses the latter using countable unions and intersections of inequalities involving these tail sums, so it belongs to every [tail sigma-algebra](../../../../../../tail-sigma-algebra.md).

The event that the partial sums are nonpositive infinitely often is **not generally a [tail event](../../../../../../tail-event.md)**. For a counterexample let $X_1$ take values $-1$ and one on a two-point [probability](../../../../../../probability.md) space, each with positive [probability](../../../../../../probability.md), and let $X_n=0$ for $n\geq2$. The event is then $\{X_1=-1\}$, while $\sigma(X_2,X_3,\ldots)$ is trivial. The variables in this example are even independent. Its status can be different for particular sequences, but it is not tail-measurable in general.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [25J](../../25j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

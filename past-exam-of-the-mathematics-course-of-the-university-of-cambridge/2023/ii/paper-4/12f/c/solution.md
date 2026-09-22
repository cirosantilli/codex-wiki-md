<h1 id="12f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Chebyshev alternation theorem](../../../../../../equioscillation-theorem.md) says that a [polynomial](../../../../../../polynomial-split.md) $P$ of [degree](../../../../../../degree-of-a-polynomial.md) at most $n$ is a [best uniform approximation](../../../../../../best-uniform-approximation.md) to $f\in C([0,1])$ if and only if there are $n+2$ points

$$
0\leq t_0<t_1<\cdots<t_{n+1}\leq1
$$

and a sign $\varepsilon\in\{1,-1\}$ for which

$$
f(t_j)-P(t_j)=\varepsilon(-1)^j\lVert f-P\rVert_\infty.
$$

This is the equiripple criterion.

To prove sufficiency, put $E=\lVert f-P\rVert_\infty$ and suppose that another polynomial $Q$ of degree at most $n$ satisfies $\lVert f-Q\rVert_\infty<E$. At every $t_j$, the difference $R=Q-P$ must have the same sign as $f-P$; hence its signs alternate at the $n+2$ ordered points. The [intermediate value theorem](../../../../../../intermediate-value-theorem.md) then gives at least one distinct root of $R$ in every interval $(t_j,t_{j+1})$, for at least $n+1$ roots in all. The [Lagrange root bound over a field](../../../../../../lagrange-root-bound-over-a-field.md) forces the nonzero polynomial $R$ to have degree at least $n+1$, contradicting $\deg R\leq n$. Therefore no $Q$ gives a smaller error, and $P$ is best.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [12F](../../12f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

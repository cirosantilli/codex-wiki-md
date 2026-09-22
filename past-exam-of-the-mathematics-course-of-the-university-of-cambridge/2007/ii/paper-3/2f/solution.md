<h1 id="2f/solution">Solution</h1>

↑ **Parent:** [2F](../2f.md)

The [polynomial](../../../../../polynomial-split.md) form of [Runge theorem](../../../../../runge-s-theorem.md) says that a function holomorphic on a neighbourhood of a compact set $K\subset\mathbb C$ with connected complement can be approximated uniformly on $K$ by [polynomials](../../../../../polynomial-split.md).

For $n\geq3$, take

$$
K_n=\{0\}\cup\{z:1/n\leq|z|\leq1-1/n,\ 0\leq\arg z\leq2\pi-1/n\}.
$$

The complement is connected: the missing angular sector connects the inner disk to the exterior, and removing the single point zero from the inner disk does not disconnect it. On a neighbourhood of the annular sector choose an analytic logarithm with arguments between $-1/(2n)$ and $2\pi-1/(2n)$. Its exponential $\exp(3\log z/2)$ agrees with the prescribed function on the sector. On a disjoint small neighbourhood of zero prescribe the analytic function zero. These two neighbourhoods define a [holomorphic function](../../../../../holomorphic-function.md) $g_n$ near $K_n$ with $g_n=f$ on $K_n$.

By [Runge theorem](../../../../../runge-s-theorem.md), choose a [polynomial](../../../../../polynomial-split.md) $p_n$ with $\sup_{K_n}|p_n-g_n|<1/n$. Every fixed nonzero point of the disk eventually belongs to all $K_n$, including points on the positive real axis; zero belongs to every $K_n$. Consequently

$$
\boxed{p_n(z)\longrightarrow f(z)\quad\text{for every }z\in D.}
$$

Each [polynomial](../../../../../polynomial-split.md) restricts to an analytic function on $D$. The excluded sector lies immediately below the positive axis and shrinks with $n$, so the construction correctly preserves the chosen value on the branch cut. It gives [pointwise convergence](../../../../../pointwise-convergence.md), not local [uniform convergence](../../../../../uniform-convergence.md) across that cut. This is [pointwise approximation by a Runge exhaustion](../../../../../pointwise-approximation-by-a-runge-exhaustion.md).

## ↑ Ancestors (10)

1. [2F](../2f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

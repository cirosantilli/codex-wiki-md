<h1 id="2f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [Runge exhaustion of a slit disk](../../../../../../runge-exhaustion-of-a-slit-disk.md), with the principal argument $-\pi<\arg z<\pi$:

$$
K_m=\{re^{i\theta}:1/m\leq r\leq1-1/m,\quad |\theta|\leq\pi-1/m\},\qquad m\geq3.
$$

These are nested compact subsets of $\Omega$. Their complements are connected: the inner disk and exterior region join through the omitted sector around the negative real radius. Every compact subset of $\Omega$ has positive distance from zero, the unit circle and the slit, so it is contained in $K_m$ for all sufficiently large $m$.

Since $f$ is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) on $\Omega$, it is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) on a neighborhood of each $K_m$. The [polynomial Runge theorem](../../../../../../polynomial-runge-theorem.md) gives $P_m$ with $\sup_{K_m}|P_m-f|<1/m$. Given any compact $K\subset\Omega$, eventually $K\subseteq K_m$, so the same estimate holds on $K$. Therefore

$$
\boxed{P_m\longrightarrow f\text{ uniformly on every compact subset of }\Omega.}
$$

The nested exhaustion makes this one sequence work simultaneously on all compact subsets.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2F](../../2f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

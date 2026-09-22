<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [first Jackson theorem for periodic approximation](../../../../../../first-jackson-theorem-for-periodic-approximation.md) asserts that a universal constant $C$ satisfies

$$
E_n^{\mathrm{trig}}(g)\le C\,\omega(g,1/n),\qquad n\ge1,
$$

for every continuous $2\pi$-periodic function $g$, where the infimum is over degree-at-most-$n$ [trigonometric polynomials](../../../../../../trigonometric-polynomial.md).

Apply it to the even function $g(\theta)=f(\cos\theta)$. If $q_n$ is a [trigonometric polynomial](../../../../../../trigonometric-polynomial.md) approximating $g$, its even part

$$
q_n^{\mathrm{ev}}(\theta)=\frac{q_n(\theta)+q_n(-\theta)}2
$$

has no larger error, because $g(-\theta)=g(\theta)$ and the triangle inequality bounds each averaged error by $\|g-q_n\|_\infty$. Every even [trigonometric polynomial](../../../../../../trigonometric-polynomial.md) has the form

$$
q_n^{\mathrm{ev}}(\theta)=\sum_{j=0}^n b_j\cos(j\theta)
=p_n(\cos\theta),\qquad
p_n(x)=\sum_{j=0}^n b_jT_j(x).
$$

Here the [Chebyshev polynomials](../../../../../../chebyshev-polynomial.md) $T_j$ have algebraic degree $j$, so $p_n$ has degree at most $n$. Surjectivity of cosine gives

$$
\|f-p_n\|_{C[-1,1]}=\|g-q_n^{\mathrm{ev}}\|_{C(\mathbb T)}.
$$

Conversely, every algebraic [polynomial](../../../../../../polynomial-split.md) of degree at most $n$ yields such an even [trigonometric polynomial](../../../../../../trigonometric-polynomial.md). Taking infima therefore proves the exact identity $E_n^{\mathrm{alg}}(f)=E_n^{\mathrm{trig}}(\widetilde f)$, not merely an inequality. Combine this with the periodic theorem and the preceding [modulus of continuity](../../../../../../modulus-of-continuity.md) estimate:

$$
\boxed{E_n^{\mathrm{alg}}(f)\le C\,\omega(\widetilde f,1/n)
\le C\,\omega(f,1/n)}.
$$

Symmetrization, the degree correspondence and the equality of norms justify every step in transferring the [Jackson-type estimate](../../../../../../jackson-type-estimate.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

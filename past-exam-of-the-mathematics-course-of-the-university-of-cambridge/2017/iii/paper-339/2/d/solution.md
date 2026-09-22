<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For each [coefficient](../../../../../../coefficient.md) index $k\geq0$, let $H_k$ have constant diagonal blocks $f_kJ$ and cross blocks $g_kJ$. The preceding block-constant argument gives $H_k\succeq0$. Define the [Hadamard powers](../../../../../../hadamard-power.md) $X^{\circ k}$, with

$$
X^{\circ0}=J_{n+m,n+m}.
$$

This is the constant entrywise power, including at zero entries; it is not the [identity matrix](../../../../../../identity-matrix.md). Repeated use of the [Schur product theorem](../../../../../../schur-product-theorem.md) shows $X^{\circ k}\succeq0$ for every $k\geq0$.

Applying the [Schur product theorem](../../../../../../schur-product-theorem.md) again makes every summand $H_k\circ X^{\circ k}$ [positive semidefinite](../../../../../../positive-semidefinite-matrix.md). The partial sums are [positive semidefinite](../../../../../../positive-semidefinite-matrix.md), and their entrywise limit is exactly $Y$. In finite [dimension](../../../../../../dimension-vector-space.md) this is a matrix-norm limit; the [positive semidefinite cone](../../../../../../positive-semidefinite-cone.md) is closed. Consequently

$$
\boxed{Y=\sum_{k=0}^\infty H_k\circ X^{\circ k}\succeq0}.
$$

Endpoint convergence follows from the stated expansions on the full interval: $f_k\geq0$ and $\sum f_k=f(1)<\infty$, while $\sum|g_k|\leq\sum f_k$. Thus the expansions converge absolutely at every [matrix](../../../../../../matrix.md) entry. This is [coefficient-dominated entrywise positivity](../../../../../../coefficient-dominated-entrywise-positivity.md).

**The [coefficient](../../../../../../coefficient.md) condition must include index zero**. We interpret the PDF's $\mathbb N$ accordingly. If it means only positive integers and no condition is imposed on $f_0,g_0$, the assertion is false: take $n=m=1$, $X=0$, $f=-1$ and $g=0$. All positive-index inequalities hold, but $Y=-I_2$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

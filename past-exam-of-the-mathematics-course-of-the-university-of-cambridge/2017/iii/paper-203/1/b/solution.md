<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $u(z)=\operatorname{Im}(z-g_A(z))$ on $D_A$. This is a [harmonic function](../../../../../../harmonic-function.md), tends to zero at infinity, and is bounded. To justify the [boundary](../../../../../../boundary-of-a-set.md) behavior without requiring a [locally connected space](../../../../../../locally-connected-space.md) as its [boundary](../../../../../../boundary-of-a-set.md), let $f_A=g_A^{-1}$. Its expansion at infinity implies that bounded $z$ cannot have $|g_A(z)|\to\infty$. If $z_n$ approaches a finite point of $\partial D_A$ and $g_A(z_n)$ had a subsequential limit inside $\mathbb H$, [continuity](../../../../../../continuous-function.md) of $f_A$ would force that point to lie inside $D_A$, a contradiction. Thus [boundary degeneration under a mapping-out function](../../../../../../boundary-degeneration-under-a-mapping-out-function.md) gives $\operatorname{Im}g_A(z_n)\to0$. Consequently $u$ extends continuously to the finite [boundary](../../../../../../boundary-of-a-set.md) with value $\operatorname{Im}z$.

Let $B$ be [planar Brownian motion](../../../../../../planar-brownian-motion.md) started at $z\in D_A$, and $\tau$ its [Brownian exit time](../../../../../../brownian-exit-time.md) from $D_A$. This time is finite almost surely: it is at most the first time the imaginary coordinate, a one-dimensional [Brownian motion](../../../../../../brownian-motion-split.md), hits zero. By the [Itô formula](../../../../../../ito-s-lemma.md), $u(B_{t\wedge\tau})$ is a bounded [martingale](../../../../../../martingale-split.md). The [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) and [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) therefore give

$$
u(z)=\mathbb E_z[u(B_\tau)]=\mathbb E_z[\operatorname{Im}B_\tau].
$$

Boundedness is important here: directly stopping the unbounded imaginary-coordinate [martingale](../../../../../../martingale-split.md) would require an unjustified [uniform integrability](../../../../../../uniform-integrability.md) assertion.

At $z=iy$, the [Laurent series](../../../../../../laurent-series.md) gives $u(iy)=a/y+O(y^{-2})$. Hence

$$
\boxed{\operatorname{hcap}(A)=\lim_{y\to\infty}y\,\mathbb E_{iy}[\operatorname{Im}B_\tau]\geq0.}
$$

The sign follows because the exit point lies on $\partial D_A\subseteq\overline{\mathbb H}$. This proves the [Brownian representation of half-plane capacity](../../../../../../brownian-representation-of-half-plane-capacity.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

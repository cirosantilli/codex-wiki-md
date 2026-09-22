<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Bonnet-Myers theorem](../../../../../../myers-s-theorem.md) states that if a complete connected $n$-dimensional [Riemannian manifold](../../../../../../riemannian-manifold.md) satisfies

$$
\operatorname{Ric}\geq(n-1)k g
$$

for some $k>0$, then

$$
\operatorname{diam}(M)\leq\frac{\pi}{\sqrt k}.
$$

In particular, $M$ is compact and has finite [fundamental group](../../../../../../fundamental-group.md).

By the [Hopf-Rinow theorem](../../../../../../hopf-rinow-theorem.md), points $p,q\in M$ are joined by a unit-speed length-minimizing [geodesic](../../../../../../geodesic.md) $\gamma:[0,\ell]\to M$. Choose a parallel orthonormal frame $E_1,\ldots,E_{n-1}$ normal to $T=\dot\gamma$ and set

$$
V_i(t)=\sin\left(\frac{\pi t}{\ell}\right)E_i(t).
$$

The endpoint-vanishing fields $V_i$ arise from fixed-endpoint variations. Since $\gamma$ minimizes length, its [Riemannian index form](../../../../../../riemannian-index-form.md) is nonnegative on each $V_i$. Summing the [second variation of Riemannian arc length](../../../../../../second-variation-of-riemannian-arc-length.md) gives

$$
0\leq\sum_{i=1}^{n-1}I(V_i,V_i)
=\int_0^\ell\left[
(n-1)\frac{\pi^2}{\ell^2}\cos^2\left(\frac{\pi t}{\ell}\right)
-\operatorname{Ric}(T,T)\sin^2\left(\frac{\pi t}{\ell}\right)
\right]dt.
$$

Using the [Ricci curvature](../../../../../../ricci-curvature.md) bound and integrating $\sin^2$ and $\cos^2$ yields

$$
0\leq\frac{(n-1)\ell}{2}\left(\frac{\pi^2}{\ell^2}-k\right),
$$

so $\ell\leq\pi/\sqrt k$. Taking the [supremum](../../../../../../supremum.md) over $p,q$ proves the diameter bound. Hopf-Rinow now makes the closed bounded space $M$ compact. Finally, the same bound applies to the complete [universal cover](../../../../../../universal-cover.md); a compact universal cover has finite fibres over $M$, so $\pi_1(M)$ is finite.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 131](../../../paper-131-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

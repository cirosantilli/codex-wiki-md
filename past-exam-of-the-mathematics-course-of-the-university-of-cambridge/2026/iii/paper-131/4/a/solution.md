<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [line in a Riemannian manifold](../../../../../../line-in-a-riemannian-manifold.md) is a unit-speed [geodesic](../../../../../../geodesic.md) $\gamma:\mathbb R\to M$ that minimizes globally:

$$
d_g(\gamma(s),\gamma(t))=|s-t|
$$

for all $s,t\in\mathbb R$. A connected noncompact manifold is [disconnected at infinity](../../../../../../disconnected-at-infinity.md) if some compact set $K$ has a complement with at least two unbounded connected components.

Choose points $p_j$ and $q_j$ in two such components with

$$
d_g(p_j,K)\to\infty,
\qquad
d_g(q_j,K)\to\infty.
$$

The [Hopf-Rinow theorem](../../../../../../hopf-rinow-theorem.md) supplies a length-minimizing geodesic $\gamma_j$ from $p_j$ to $q_j$. Its image must meet $K$, since otherwise it would connect the two different components of $M\setminus K$. Reparametrize so that $\gamma_j(0)=x_j\in K$. After taking a subsequence, compactness gives $x_j\to x\in K$ and the unit tangent vectors $\dot\gamma_j(0)$ converge to some unit $v\in T_xM$.

Both endpoint parameters tend to infinity because their distances from $K$ do. Smooth dependence of geodesics on initial data therefore makes $\gamma_j$ converge on every compact parameter interval to the complete geodesic

$$
\gamma(t)=\exp_x(tv).
$$

Every finite segment of every $\gamma_j$ minimizes length. Passing to the limit gives $d_g(\gamma(s),\gamma(t))=|s-t|$, so $\gamma$ is a line.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 131](../../../paper-131-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

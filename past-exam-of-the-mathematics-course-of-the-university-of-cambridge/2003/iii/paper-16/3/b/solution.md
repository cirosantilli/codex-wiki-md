<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $t_0$ be the finite cut time and put $q=\gamma(t_0)$. Continuity of [Riemannian distance](../../../../../../riemannian-distance.md) shows that the segment to $q$ still minimizes and $d(p,q)=t_0$. Choose $t_j\downarrow t_0$ with $t_j>t_0$. By the [Hopf-Rinow theorem](../../../../../../hopf-rinow-theorem.md), there is a minimizing [geodesic](../../../../../../geodesic.md) from $p$ to $q_j=\gamma(t_j)$ with length $\ell_j=d(p,q_j)<t_j$ and initial unit vector $v_j$. Continuity gives $\ell_j\to t_0$.

The unit tangent sphere is compact, so after a subsequence $v_j\to v$. Smooth dependence of the [Riemannian exponential map](../../../../../../exponential-map-riemannian-geometry.md) gives $\exp_p(t_0v)=q$. The [geodesic](../../../../../../geodesic.md) with initial vector $v$ has length $t_0=d(p,q)$ up to $q$, hence minimizes. If $v\ne\dot\gamma(0)$, this is the required second minimizing [geodesic](../../../../../../geodesic.md).

Suppose instead $v=\dot\gamma(0)$ and $q$ is not a [conjugate point](../../../../../../conjugate-point.md). Then the [differential](../../../../../../differential-of-a-smooth-map.md) of $\exp_p$ at $t_0\dot\gamma(0)$ is nonsingular. The [inverse function theorem](../../../../../../inverse-function-theorem.md) makes $\exp_p$ injective on a neighborhood of this vector. For large $j$, both $\ell_jv_j$ and $t_j\dot\gamma(0)$ belong to that neighborhood and exponentiate to $q_j$. They must be equal, implying $\ell_j=t_j$, a contradiction. Thus either a distinct minimizing [geodesic](../../../../../../geodesic.md) exists or $q$ is conjugate. In the latter case it is the first [conjugate point](../../../../../../conjugate-point.md), since part (a) excludes any earlier one on a minimizing segment. We have proved the **cut-point dichotomy for complete Riemannian manifolds**.

Here the relevant concept is a [Riemannian cut point](../../../../../../riemannian-cut-point.md), not the topological [cut point](../../../../../../cut-point.md) obtained by disconnecting a space through removal of a point.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

By the [Hodge decomposition theorem](../../../../../../hodge-decomposition-theorem.md), the first [Betti number](../../../../../../betti-number.md) is $b_1(M)=\dim\mathcal H^1(M)$. Part (b) makes every element of this space a [parallel differential form](../../../../../../parallel-differential-form.md). For any fixed $p\in M$, consider the linear evaluation map

$$
\operatorname{ev}_p:\mathcal H^1(M)\longrightarrow T_p^*M,\qquad\omega\longmapsto\omega_p.
$$

It is injective. A parallel form with $\omega_p=0$ remains zero under [parallel transport](../../../../../../parallel-transport.md) along any path from $p$; [connectedness](../../../../../../connected-space.md) of the [smooth manifold](../../../../../../smooth-manifold.md) makes every point reachable by such a path. Equivalently, the derivative of the squared norm of a parallel form is zero in every direction, so its norm is constant on the connected manifold. Either argument gives $\omega=0$ globally. Since $\dim T_p^*M=n$, the [dimension bound for harmonic one-forms under nonnegative Ricci curvature](../../../../../../dimension-bound-for-harmonic-one-forms-under-nonnegative-ricci-curvature.md) gives

$$
\boxed{b_1(M)\le n.}
$$

For an explicit obstruction in dimension three, take $N=\Sigma_2\times S^1$, where $\Sigma_2$ is a closed orientable surface of genus two. It is a compact connected smooth three-manifold. A cell decomposition of $\Sigma_2$ has one vertex, four one-cells and one two-cell attached by a product of commutators. Its cellular boundary into the one-cells is zero, because each generator has total exponent zero in that attaching word; the boundary of every one-cell is also zero. Therefore $H^1(\Sigma_2;\mathbb R)=\mathbb R^4$. The [Künneth theorem](../../../../../../kunneth-theorem.md) in degree one and $H^1(S^1;\mathbb R)=\mathbb R$ give

$$
H^1(N;\mathbb R)\cong H^1(\Sigma_2;\mathbb R)\oplus H^1(S^1;\mathbb R)\cong\mathbb R^5.
$$

Consequently

$$
\boxed{\dim N=3,\qquad b_1(N)=5>3,\qquad
N\text{ admits no metric with }\operatorname{Ric}\ge0.}
$$

This is the [Betti-number obstruction to nonnegative Ricci curvature](../../../../../../betti-number-obstruction-to-nonnegative-ricci-curvature.md). It rules out every [Riemannian metric](../../../../../../riemannian-metric.md) on that underlying manifold, not merely a particular product metric.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

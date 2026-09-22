<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the sign convention in the supplied scalar [Laplace-Beltrami operator](../../../../../../laplace-beltrami-operator.md) identity, and let $X=\omega^\sharp$ be the metric-dual [vector field](../../../../../../vector-field.md). Integrate that [Bochner formula for one-forms](../../../../../../bochner-weitzenbock-formula-for-one-forms.md) over the closed [Riemannian manifold](../../../../../../riemannian-manifold.md), with its volume density $dV_g$. The integral of a scalar Laplacian is zero: on an oriented manifold this is the [Riemannian divergence theorem](../../../../../../riemannian-divergence-theorem.md) applied to its gradient, and the same density formula is valid without orientability. Hence

$$
0=\int_M\left(|\nabla\omega|^2+\operatorname{Ric}(X,X)\right)dV_g.
$$

Both terms are nonnegative, because $\operatorname{Ric}\ge0$. The smooth nonnegative integrand must therefore vanish everywhere: a strictly positive value would remain positive on an open neighborhood of positive volume and make its integral positive. In particular $|\nabla\omega|^2=0$ at every point, proving

$$
\boxed{\nabla\omega=0.}
$$

Thus [harmonic one-forms are parallel under nonnegative Ricci curvature](../../../../../../harmonic-one-forms-are-parallel-under-nonnegative-ricci-curvature.md). The same argument also gives $\operatorname{Ric}(X,X)=0$ pointwise. No [orientation](../../../../../../orientation-of-a-simplex.md) or [connectedness](../../../../../../connected-space.md) assumption is needed for this step.

## ↑ Ancestors (11)

1. [B](../b.md)
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

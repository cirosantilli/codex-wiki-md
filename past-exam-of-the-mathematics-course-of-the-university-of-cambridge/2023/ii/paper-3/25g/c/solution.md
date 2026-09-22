<h1 id="25g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At $p$, the surface $\widetilde S$ cannot cross the boundary $S=\partial\mathcal R$, because it lies inside $\mathcal R$. Consequently the two surfaces are tangent at $p$. Apply a [proper Euclidean motion of Euclidean three-space](../../../../../../proper-euclidean-motion-of-euclidean-three-space.md) so that $p=0$, their common tangent plane is $z=0$, and the prescribed inward [unit normal](../../../../../../unit-normal.md) is $N=e_3$. Locally write

$$
S:\ z=f(x,y),
\qquad
\widetilde S:\ z=g(x,y),
$$

with the region $\mathcal R$ on the side $z\geq f(x,y)$. Then

$$
g\geq f,
\qquad
g(0)=f(0),
\qquad
\nabla g(0)=\nabla f(0)=0.
$$

Thus $g-f$ has a [local minimum](../../../../../../local-minimum.md) at zero and its [Hessian matrix](../../../../../../hessian-matrix.md) is [positive semidefinite](../../../../../../positive-semidefinite-matrix.md). The [fundamental forms of a graph surface](../../../../../../fundamental-forms-of-a-graph-surface.md) at a horizontal tangent plane give

$$
H(0)=\frac12\operatorname{tr}\operatorname{Hess}f(0),
\qquad
\widetilde H(0)=\frac12\operatorname{tr}\operatorname{Hess}g(0).
$$

Taking the trace of the positive-semidefinite difference proves the [mean-curvature comparison at tangential contact](../../../../../../mean-curvature-comparison-at-tangential-contact.md):

$$
\boxed{\widetilde H(p)\geq H(p).}
$$

There is no analogous conclusion for $K$. In the same local coordinates take

$$
f(x,y)=-x^2-y^2,
\qquad
g(x,y)=-\frac12(x^2+y^2).
$$

Then $g\geq f$, so the second graph lies on the inward side of the first, while the [Gaussian curvature of a graph surface](../../../../../../gaussian-curvature-of-a-graph-surface.md) gives

$$
H_f(0)=-2,
\qquad H_g(0)=-1,
\qquad
K_f(0)=4,
\qquad K_g(0)=1.
$$

Hence the mean-curvature inequality holds but

$$
\boxed{\widetilde K(p)<K(p).}
$$

Using smooth bump functions, these local graph patches can be completed away from $p$ to a compact region with connected smooth boundary and a closed interior surface without changing their germs at $p$. This realizes the [counterexample](../../../../../../gaussian-curvature-has-no-tangential-contact-comparison-principle.md) under the global hypotheses.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [25G](../../25g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume a [classical solution](../../../../../classical-solution.md) $u\in C^2(D)\cap C(\overline D)$, as needed to interpret the boundary values. At an interior local minimum its [Hessian](../../../../../hessian-matrix.md) is [positive semidefinite](../../../../../positive-semidefinite-matrix.md), hence $\Delta u\geq0$. But the equation gives $\Delta u=-e^{-x^2}<0$, a contradiction. Since $D$ is bounded and $u=0$ on its boundary, a nonpositive interior value would either furnish an interior negative minimum or itself be a zero minimum. Thus $\boxed{u>0\text{ in }D}$.

For the upper bound use the barrier $w(x,y)=(1-x^2-y^2)/4$, which satisfies $-\Delta w=1$. Set $z=w-u$. On the boundary $z=w\geq0$, because the domain lies inside the unit disk, while

$$
-\Delta z=1-e^{-x^2}\geq0.
$$

The [quadratic perturbation proof of the minimum principle](../../../../../quadratic-perturbation-proof-of-the-minimum-principle.md) gives $z\geq0$. The [strong minimum principle for elliptic operators](../../../../../strong-minimum-principle-for-elliptic-operators.md) makes this strict in the connected interior unless $z$ is constant. Constancy is impossible since $1-e^{-x^2}$ is not identically zero on any open domain. Hence

$$
\boxed{0<u(x,y)<\tfrac14(1-x^2-y^2)\quad\text{throughout }D.}
$$

This last strong-principle step handles points with $x=0$, where the comparison forcing itself vanishes. Simple connectedness is not needed for the comparison argument.

With source point $\xi\in D$ and field point $X=(x,y)$, the [Dirichlet Green function](../../../../../dirichlet-green-function.md) for the operator $-\Delta$ satisfies

$$
\boxed{-\Delta_XG(X,\xi)=\delta_\xi(X)\text{ in }D,\qquad G(X,\xi)=0\text{ on }\partial D.}
$$

Classically it is harmonic off $\xi$, with the two-dimensional normalization $G(X,\xi)=-(2\pi)^{-1}\log|X-\xi|+H(X,\xi)$, where $H$ is regular near the source. Equivalently $-\lim_{r\downarrow0}\int_{|X-\xi|=r}\partial_rG\,ds=1$. This sign convention gives the representation $u(X)=\int_DG(X,\xi)e^{-\xi_1^2}\,d\xi$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the differential equations and applications course of the University of Oxford](../../../../split.md)
6. [Differential equations and applications course of the University of Oxford](../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

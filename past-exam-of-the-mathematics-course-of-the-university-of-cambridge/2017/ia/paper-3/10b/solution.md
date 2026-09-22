<h1 id="10b/solution">Solution</h1>

↑ **Parent:** [10B](../10b.md)

Let $a$ be any constant [vector](../../../../../vector.md) and take $u=\phi a$. The [product rule for divergence](../../../../../product-rule-for-divergence.md) gives $\nabla\cdot u=a\cdot\nabla\phi$. The [divergence theorem](../../../../../divergence-theorem.md) on a bounded region with piecewise smooth boundary, oriented outward, therefore yields

$$
a\cdot\int_V\nabla\phi\,dV=a\cdot\int_S\phi\,d\mathbf S.
$$

Since $a$ is arbitrary, equality of all components proves

$$
\boxed{\int_V\nabla\phi\,dV=\int_S\phi\,d\mathbf S.}
$$

Here $\phi$ is [continuously differentiable](../../../../../continuously-differentiable-function.md) on a neighbourhood of the closed region.

For the side of this [right circular cone](../../../../../right-circular-cone.md), the parameter tangents are $x_r=(\cos\theta,\sin\theta,\sqrt3)$ and $x_\theta=(-r\sin\theta,r\cos\theta,0)$. Their [cross product](../../../../../cross-product.md) in the outward order is

$$
\boxed{d\mathbf S=(x_\theta\times x_r)\,dr\,d\theta
=(\sqrt3\cos\theta,\sqrt3\sin\theta,-1)r\,dr\,d\theta.}
$$

The sign is outward because the solid [right circular cone](../../../../../right-circular-cone.md) lies at smaller cylindrical radius for fixed height. Reversing the parameter order reverses the [oriented surface element](../../../../../oriented-surface-element.md).

To check the integral identity, the closed boundary must include the top [Euclidean disk](../../../../../disk-mathematics.md) $z=1$, radius $1/\sqrt3$, as well as the curved side. For $\phi=z^2$, horizontal components cancel on integrating $\theta$. The side contribution is

$$
\int_{\rm side}\phi\,d\mathbf S
=-2\pi\int_0^{1/\sqrt3}3r^3\,dr\,e_z
=-\frac\pi6e_z.
$$

On the top [Euclidean disk](../../../../../disk-mathematics.md) $\phi=1$ and $d\mathbf S=e_z\,dA$, so its contribution is $(\pi/3)e_z$. The total is $(\pi/6)e_z$. Independently, the cross-section of the solid at height $z$ has area $\pi z^2/3$, and $\nabla\phi=2ze_z$, giving

$$
\int_V\nabla\phi\,dV
=\int_0^1 2z\frac{\pi z^2}{3}\,dz\,e_z
=\boxed{\frac\pi6e_z}.
$$

Thus the two sides agree. The curved side alone is not a closed surface and does not satisfy this volume identity. The apex has zero area; alternatively one can truncate at height $\varepsilon$ and let $\varepsilon\downarrow0$, with the extra boundary contribution vanishing.

## ↑ Ancestors (10)

1. [10B](../10b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

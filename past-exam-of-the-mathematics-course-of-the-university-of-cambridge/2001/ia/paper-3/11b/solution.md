<h1 id="11b/solution">Solution</h1>

↑ **Parent:** [11B](../11b.md)

The [divergence theorem](../../../../../divergence-theorem.md) states that a continuously differentiable [vector field](../../../../../vector-field.md) on a bounded region $V$ satisfies

$$
\int_V\nabla\cdot\mathbf u\,dV=\int_{\partial V}\mathbf u\cdot\mathbf n\,dS,
$$

with outward [unit normal](../../../../../unit-normal.md) $\mathbf n$ and a sufficiently regular boundary; piecewise smooth boundaries are also allowed. For $\mathbf u=\mathbf c\,\Omega$ with constant $\mathbf c$, the left side is $\mathbf c\cdot\int_V\nabla\Omega\,dV$ and the right side is $\mathbf c\cdot\int_{\partial V}\Omega\mathbf n\,dS$. Equality for every constant vector gives the [gradient volume-to-boundary identity](../../../../../gradient-volume-to-boundary-identity.md)

$$
\boxed{\int_V\nabla\Omega\,dV=\int_{\partial V}\Omega\,d\mathbf S.}
$$

For the cone and its cap, the volume has $0\le z\le1$ and $0\le r\le\sqrt3z$ in [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md). Its volume is $\int_0^1\pi(\sqrt3z)^2\,dz=\pi$. Since $\nabla\Omega=-\mathbf e_z$,

$$
\int_V\nabla\Omega\,dV=-\pi\mathbf e_z.
$$

The cap at $z=1$ has area $3\pi$, outward normal $\mathbf e_z$ and $\Omega=a-1$, so its contribution to the [surface integral](../../../../../surface-integral.md) is $3\pi(a-1)\mathbf e_z$.

Parameterize the side by $\mathbf R(r,\theta)=(r\cos\theta,r\sin\theta,r/\sqrt3)$, $0\le r\le\sqrt3$, $0\le\theta<2\pi$. The outward [vector area element](../../../../../vector-area-element.md) is

$$
d\mathbf S=(\mathbf R_\theta\times\mathbf R_r)\,dr\,d\theta
=\left(\frac r{\sqrt3}\mathbf e_r-r\mathbf e_z\right)dr\,d\theta,
$$

pointing radially outward and downward from the region above the cone. The radial part integrates to zero around the circle. The vertical part of the side integral is

$$
-2\pi\int_0^{\sqrt3}\left(a-\frac r{\sqrt3}\right)r\,dr\,\mathbf e_z
=(-3\pi a+2\pi)\mathbf e_z.
$$

Adding cap and side gives

$$
\boxed{\int_{\partial V}(a-z)\,d\mathbf S
=\{3\pi(a-1)-3\pi a+2\pi\}\mathbf e_z
=-\pi\mathbf e_z
=\int_V\nabla(a-z)\,dV.}
$$

The apex and circular rim have zero surface area. Alternatively, removing a tiny apex neighborhood and taking its radius to zero justifies applying the smooth-boundary theorem there; the additional flux vanishes because the scalar field is bounded.

## ↑ Ancestors (10)

1. [11B](../11b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="9a/solution">Solution</h1>

↑ **Parent:** [9A](../9a.md)

In [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md), $\rho=(x^2+y^2)^{1/2}$ and $\mathbf F=(f(\rho)x/\rho,f(\rho)y/\rho,0)$. The [chain rule](../../../../../chain-rule.md) gives $\partial_x\rho=x/\rho$ and $\partial_y\rho=y/\rho$. Therefore

$$
\boxed{\begin{aligned}
\frac{\partial F_1}{\partial x}&=f'(\rho)\cos^2\phi+\frac{f(\rho)}\rho\sin^2\phi,\\
\frac{\partial F_2}{\partial y}&=f'(\rho)\sin^2\phi+\frac{f(\rho)}\rho\cos^2\phi,\\
\frac{\partial F_3}{\partial z}&=0,\qquad
\nabla\cdot\mathbf F=f'(\rho)+\frac{f(\rho)}\rho.
\end{aligned}}
$$

This is [cylindrically radial divergence](../../../../../cylindrically-radial-divergence.md), valid for $\rho>0$.

The bounded domain is outside the unit cylinder, below the inverse-square surface and above the lower plane:

$$
V=\left\{\frac14\le z\le1,\quad 1\le\rho\le z^{-1/2},\quad0\le\phi<2\pi\right\}
=\left\{1\le\rho\le2,\quad\frac14\le z\le\rho^{-2}\right\}.
$$

The upper plane touches only the rim $\rho=1,z=1$; it is not an extra positive-area top face. Revolving the shaded meridional region below around the $z$ axis gives the three-dimensional domain.

<a id="9a/image-meridional-section-of-the-annular-volume-between-the-unit-cylinder-inverse-square-surface-and-lower-plane"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-3-domain.png)

**[Figure 1](#9a/image-meridional-section-of-the-annular-volume-between-the-unit-cylinder-inverse-square-surface-and-lower-plane). Meridional section of the annular volume between the unit cylinder, inverse-square surface and lower plane**.

With the [Jacobian determinant](../../../../../jacobian-determinant.md) $dV=\rho\,d\rho\,d\phi\,dz$ of [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md),

$$
\boxed{\operatorname{Vol}(V)=\pi\int_{1/4}^1(z^{-1}-1)\,dz=\pi\left(\log4-\frac34\right).}
$$

Zero [divergence](../../../../../divergence.md) gives $(\rho f)'=0$, hence the most general solution on the positive radial interval is

$$
\boxed{f(\rho)=\frac A\rho,\qquad A\in\mathbb R.}
$$

Although this [vector field](../../../../../vector-field.md) is singular on the axis if $A\ne0$, the entire closure of $V$ lies at $\rho\ge1$, so it is smooth on a neighbourhood of $V$ and the [divergence theorem](../../../../../divergence-theorem.md) applies.

Its volume integral of [divergence](../../../../../divergence.md) is zero. Compute the outward [surface integral](../../../../../surface-integral.md) directly. On the inner cylinder, $\mathbf n=-\mathbf e_\rho$, $dS=d\phi\,dz$, and the flux is $-2\pi A(1-1/4)=-3\pi A/2$. On the curved roof $z=g(\rho)=\rho^{-2}$, the outward [vector surface element of a graph](../../../../../vector-surface-element-of-a-graph.md) is

$$
d\mathbf S=(-g'(\rho)\mathbf e_\rho+\mathbf e_z)\rho\,d\rho\,d\phi
=\left(\frac2{\rho^2}\mathbf e_\rho+\rho\mathbf e_z\right)d\rho\,d\phi.
$$

Therefore its flux is

$$
\int_0^{2\pi}\int_1^2\frac{2A}{\rho^3}\,d\rho\,d\phi=\frac{3\pi A}{2}.
$$

The horizontal bottom has zero flux and the top rim has zero surface area. Summing gives

$$
\boxed{\int_{\partial V}\mathbf F\cdot d\mathbf S=0=\int_V\nabla\cdot\mathbf F\,dV,}
$$

which verifies the [divergence theorem](../../../../../divergence-theorem.md) with every boundary contribution accounted for.

## ↑ Ancestors (10)

1. [9A](../9a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

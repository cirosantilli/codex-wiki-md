<h1 id="10c/solution">Solution</h1>

↑ **Parent:** [10C](../10c.md)

The [divergence theorem](../../../../../divergence-theorem.md) states that a continuously differentiable [vector field](../../../../../vector-field.md) on a bounded region with piecewise smooth boundary satisfies

$$
\int_V\nabla\cdot\mathbf u\,dV=\int_{\partial V}\mathbf u\cdot\mathbf n\,dS,
$$

with the unit normal pointing out of $V$. Apply it separately to $\mathbf u=f\mathbf e_i$, where $\mathbf e_i$ is each constant Cartesian basis vector. Since $\nabla\cdot(f\mathbf e_i)=\partial_i f$ and $(f\mathbf e_i)\cdot\mathbf n=fn_i$, the three component identities combine to give

$$
\boxed{\int_V\nabla f\,dV=\int_{\partial V}f\,d\mathbf S.}
$$

For the specified [scalar field](../../../../../scalar-field.md), $\nabla f=(z,0,x)$. The $x$ term integrates to zero by reflection symmetry. At height $z$, the region has a disk cross-section of area $\pi(a^2-cz)$, and $0\leq z\leq a^2/c$. Therefore the [volume integral](../../../../../volume-integral.md) is

$$
\int_V\nabla f\,dV
=\mathbf e_x\pi\int_0^{a^2/c}z(a^2-cz)\,dz
=\boxed{\frac{\pi a^6}{6c^2}\mathbf e_x.}
$$

To check the [surface integral](../../../../../surface-integral.md) independently, split the boundary into the base disk and the curved graph $z=g(x,y)=(a^2-x^2-y^2)/c$. On the base $f=0$, so its contribution vanishes. The region lies below the curved graph, whose outward [vector surface element of a graph](../../../../../vector-surface-element-of-a-graph.md) is

$$
d\mathbf S=(-g_x,-g_y,1)\,dx\,dy=\left(\frac{2x}{c},\frac{2y}{c},1\right)dx\,dy.
$$

Over the disk $x^2+y^2\leq a^2$, the $y$ and $z$ components of $f\,d\mathbf S$ are odd in $x$ and integrate to zero. Its $x$ component gives, in [polar coordinates](../../../../../polar-coordinates.md),

$$
\begin{aligned}
\int_{\partial V}f\,d\mathbf S
&=\frac{2\mathbf e_x}{c^2}\int_{x^2+y^2\leq a^2}x^2(a^2-x^2-y^2)\,dx\,dy\\
&=\frac{2\mathbf e_x}{c^2}\int_0^{2\pi}\cos^2\phi\,d\phi\int_0^a s^3(a^2-s^2)\,ds\\
&=\frac{\pi a^6}{6c^2}\mathbf e_x.
\end{aligned}
$$

Thus the two explicitly evaluated integrals agree, with the outward orientation included.

## ↑ Ancestors (10)

1. [10C](../10c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

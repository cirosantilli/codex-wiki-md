<h1 id="3b/solution">Solution</h1>

↑ **Parent:** [3B](../3b.md)

For an arbitrary constant vector $\mathbf c$, the [product rule for divergence](../../../../../product-rule-for-divergence.md) gives

$$
\nabla\mathbin{\cdot}(\phi\mathbf c)=\mathbf c\mathbin{\cdot}\nabla\phi.
$$

The [divergence theorem](../../../../../divergence-theorem.md) therefore implies

$$
\mathbf c\mathbin{\cdot}\int_V\nabla\phi\,dV
=\int_V\nabla\mathbin{\cdot}(\phi\mathbf c)\,dV
=\int_S\phi\,\mathbf c\mathbin{\cdot}d\mathbf S
=\mathbf c\mathbin{\cdot}\int_S\phi\,d\mathbf S.
$$

Since this holds for every $\mathbf c$,

$$
\boxed{\int_V\nabla\phi\,dV=\int_S\phi\,d\mathbf S}.
$$

For $\phi=x+y$, $\nabla\phi=(1,1,0)$. The ball of radius $a$ has volume $4\pi a^3/3$, so

$$
\int_V\nabla\phi\,dV=\frac{4\pi a^3}{3}(1,1,0).
$$

On the sphere, use $x=a\sin\theta\cos\varphi$, $y=a\sin\theta\sin\varphi$ and the stated outward [oriented surface element](../../../../../oriented-surface-element.md). The first component of the surface integral is

$$
a^3\int_0^\pi\sin^3\theta\,d\theta
\int_0^{2\pi}(\cos^2\varphi+\sin\varphi\cos\varphi)\,d\varphi
=a^3\frac43\pi,
$$

and symmetry gives the same second component and a zero third component. The two sides agree.

## ↑ Ancestors (10)

1. [3B](../3b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

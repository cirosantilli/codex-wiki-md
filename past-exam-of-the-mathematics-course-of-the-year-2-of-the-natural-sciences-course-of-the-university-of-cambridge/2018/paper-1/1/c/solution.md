<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First compute the [curl](../../../../../curl.md) directly:

$$
\nabla\times\mathbf F=(0,1,2x).
$$

Reflection symmetry in $x$ makes the last component integrate to zero. The middle component gives the [hemisphere](../../../../../hemisphere.md)'s volume, so

$$
\int_V\nabla\times\mathbf F\,dV
=\left(0,\frac{2\pi R^3}{3},0\right).
$$

For an independent [surface integral](../../../../../surface-integral.md), the closed boundary consists of the curved [hemisphere](../../../../../hemisphere.md) and its flat base. The right-hand side in part (b) is $\int_S\mathbf n\times\mathbf F\,dS$.

On the curved part use [spherical coordinates](../../../../../spherical-coordinate-system.md) with $0\leq\theta\leq\pi/2$ and $0\leq\phi<2\pi$. There,

$$
\begin{aligned}
\mathbf n&=(\sin\theta\cos\phi,\sin\theta\sin\phi,\cos\theta),\\
\mathbf F&=(R\cos\theta,R^2\sin^2\theta,0),\qquad dS=R^2\sin\theta\,d\theta\,d\phi,\\
\mathbf n\times\mathbf F
&=(-R^2\cos\theta\sin^2\theta,\ R\cos^2\theta,R^2\sin^3\theta\cos\phi-R\sin\theta\cos\theta\sin\phi).
\end{aligned}
$$

The last component has zero angular integral. The first two components give

$$
\int_{S_{\mathrm{curved}}}\mathbf n\times\mathbf F\,dS
=\left(-2\pi R^4\int_0^{\pi/2}\cos\theta\sin^3\theta\,d\theta,
2\pi R^3\int_0^{\pi/2}\cos^2\theta\sin\theta\,d\theta,0\right)
=\left(-\frac{\pi R^4}{2},\frac{2\pi R^3}{3},0\right).
$$

On the base, $z=0$ and the outward [normal vector](../../../../../normal-vector.md) is $-\mathbf e_z$. Thus $\mathbf n\times\mathbf F=(x^2+y^2,0,0)$. In [polar coordinates](../../../../../polar-coordinates.md) its integral is

$$
\int_{S_{\mathrm{base}}}\mathbf n\times\mathbf F\,dS
=\left(2\pi\int_0^R\rho^3\,d\rho,0,0\right)
=\left(\frac{\pi R^4}{2},0,0\right).
$$

The first components cancel, and therefore both required sides equal

$$
\boxed{\left(0,\frac{2\pi R^3}{3},0\right),\qquad \alpha=\frac{2\pi R^3}{3}}.
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

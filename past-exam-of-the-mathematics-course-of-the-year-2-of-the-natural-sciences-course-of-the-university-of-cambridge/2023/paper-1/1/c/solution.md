<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $a=\sinh1$ and $c=\cosh1$. The region is the first-octant portion of the [ellipsoid](../../../../../ellipsoid.md) $(x^2+y^2)/a^2+z^2/c^2\leq1$. In [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md), write $\rho=\sqrt{x^2+y^2}$ and $0\leq\phi\leq\pi/2$. Away from the axis, the [divergence](../../../../../divergence.md) is

$$
\nabla\cdot\mathbf F=\frac{2x+2y}{x^2+y^2}+\frac1\rho=\frac{2\cos\phi+2\sin\phi+1}{\rho}.
$$

The field is singular on the axis, so applying the classical [divergence theorem](../../../../../divergence-theorem.md) there without qualification would be invalid. Instead remove $\rho<\varepsilon$ and apply it to the remaining region. On the added cylindrical boundary the [unit normal](../../../../../unit-normal.md) is $-\mathbf e_\rho$, and

$$
\mathbf F\cdot(-\mathbf e_\rho)=-\log(\varepsilon^2)(\cos\phi+\sin\phi).
$$

Its area element is $\varepsilon\,d\phi\,dz$, so its [flux](../../../../../flux.md) is $O(\varepsilon|\log\varepsilon|)\to0$. The axial component of the field has zero [dot product](../../../../../dot-product.md) with this normal. The [volume integral](../../../../../volume-integral.md) of the [divergence](../../../../../divergence.md) is locally integrable, because its $1/\rho$ factor cancels the cylindrical measure. Thus [removing a singular axis in a flux integral](../../../../../removing-a-singular-axis-in-a-flux-integral.md) gives the desired improper [surface integral](../../../../../surface-integral.md) with no extra axial term.

The [divergence theorem](../../../../../divergence-theorem.md) now reduces the calculation to

$$
\begin{aligned}
I&=\int_0^{\pi/2}(2\cos\phi+2\sin\phi+1)\,d\phi\int_0^c\int_0^{a\sqrt{1-z^2/c^2}}d\rho\,dz\\
&=\left(4+\frac\pi2\right)ac\int_0^1\sqrt{1-s^2}\,ds\\
&=\left(4+\frac\pi2\right)\frac{\pi ac}{4}
=\boxed{\frac{\pi(8+\pi)}8\sinh1\cosh1=\frac{\pi(8+\pi)}{16}\sinh2.}
\end{aligned}
$$

The integral over $s$ is the area of a quarter unit disk. All boundary [fluxes](../../../../../flux.md) are interpreted as convergent [improper integrals](../../../../../improper-integral.md) at the axis.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

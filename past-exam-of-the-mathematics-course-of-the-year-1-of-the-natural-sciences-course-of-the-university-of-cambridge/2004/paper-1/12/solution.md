<h1 id="12/solution">Solution</h1>

↑ **Parent:** [12](../12.md)

Use [cylindrical coordinates](../../../../cylindrical-coordinate-system.md) with $dV=r\,dr\,d\theta\,dz$, $0\leq\theta<2\pi$, $0\leq z\leq h$ and $0\leq r\leq a(1-z/h)$. Set $s=1-z/h$. Integrating first over radius gives the mass per unit height

$$
\frac{dM}{dz}=2\pi\rho_0\left[\frac{a^2s^2}{2}+\frac{a^2s^3}{3}\right]=\pi\rho_0a^2\left(s^2+\frac23s^3\right).
$$

Therefore

$$
\boxed{M=\pi\rho_0a^2h\int_0^1\left(s^2+\frac23s^3\right)ds=\frac12\pi\rho_0a^2h.}
$$

For the first moment about the base, use $z=h(1-s)$:

$$
Md=\pi\rho_0a^2h^2\int_0^1(1-s)\left(s^2+\frac23s^3\right)ds=\frac7{60}\pi\rho_0a^2h^2.
$$

Dividing by the total mass gives

$$
\boxed{d=\frac{7h}{30}.}
$$

The [center of mass of a cone with a power-law radial density](../../../../center-of-mass-of-a-cone-with-a-power-law-radial-density.md) gives an independent decomposition: the uniform-density component has centroid $h/4$, while the component proportional to $r$ has centroid $h/5$ and half as much mass. Their mass-weighted mean is $7h/30$. Density increasing toward the wider outer parts consequently moves the center below the uniform cone's $h/4$.

## ↑ Ancestors (12)

1. [12](../12.md)
2. [Paper 1](../../paper-1-split.md)
3. [2004](../../split.md)
4. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

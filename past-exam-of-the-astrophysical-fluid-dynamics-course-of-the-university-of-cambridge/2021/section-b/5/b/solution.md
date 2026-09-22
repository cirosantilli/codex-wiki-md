<h1 id="section-b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $\rho=\rho_c e^{-\Psi(\xi)}$ and $r=a\xi$. Then $d\ln\rho/dr=-a^{-1}\Psi'$ and the equation from part (a) becomes

$$
-\frac1{a^2\xi^2}\frac d{d\xi}(\xi^2\Psi')
=-\frac{4\pi G\rho_c}{K}e^{-\Psi}.
$$

With $a^2=K/(4\pi G\rho_c)$, the coefficients cancel, giving the [isothermal Lane-Emden equation](../../../../../isothermal-lane-emden-equation.md)

$$
\boxed{\frac1{\xi^2}\frac d{d\xi}(\xi^2\Psi')=e^{-\Psi}.}
$$

The regular central [boundary conditions](../../../../../boundary-condition.md) are

$$
\boxed{\Psi(0)=0,\qquad\Psi'(0)=0.}
$$

The first makes the central [mass density](../../../../../density.md) equal to $\rho_c$. The second follows from smooth [spherical symmetry](../../../../../spherical-symmetry.md) and the vanishing central [gravitational acceleration](../../../../../gravitational-acceleration.md); a preferred radial slope at the origin would be singular. Substitution of a regular [power series](../../../../../power-series.md) gives

$$
\Psi(\xi)=\frac{\xi^2}{6}-\frac{\xi^4}{120}+O(\xi^6),
$$

which supplies nonsingular starting data for numerical integration. The central conditions select the regular solution, not the [singular isothermal sphere](../../../../../singular-isothermal-sphere.md).

## ↑ Ancestors (14)

1. [B](../b.md)
2. [5](../../5.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../../split.md)
6. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)

<h1 id="2/grounded-hemisphere/solution">Solution</h1>

↑ **Parent:** [Grounded hemisphere](../grounded-hemisphere.md)

Reflect the source across the equatorial plane and subtract the two ball kernels. This gives the [Dirichlet Green function inside a hemisphere](../../../../../dirichlet-green-function-inside-a-hemisphere.md) $G_{\rm hemi}(\mathbf x;\mathbf x_0)=G_B(\mathbf x;\mathbf x_0)-G_B(\mathbf x;\mathbf x_0^-)$. It is zero on the spherical boundary because each ball kernel is zero there, and on the plane because reflection makes their values equal.

For a [point charge](../../../../../point-charge.md) $e$, [Poisson's equation](../../../../../poisson-s-equation.md) in SI units is $\Delta V=-e\delta(\mathbf x-\mathbf x_0)/\varepsilon_0$, so $V=-eG_{\rm hemi}/\varepsilon_0$. Writing $\mathbf x_0^{*-}$ for the reflected inverse point gives

$$
\boxed{V(\mathbf x)=\frac{e}{4\pi\varepsilon_0}\left[\frac1{|\mathbf x-\mathbf x_0|}-\frac1{|\mathbf x-\mathbf x_0^-|}-\frac{a/r_0}{|\mathbf x-\mathbf x_0^*|}+\frac{a/r_0}{|\mathbf x-\mathbf x_0^{*-}|}\right].}
$$

The construction uses the real charge, its negative reflected image, a negative inversion image of magnitude $ea/r_0$, and its positive reflected image. Reflection and inversion commute. All three images lie outside the open upper half-ball, and the prescribed zero boundary values determine the [electrostatic potential](../../../../../electric-potential.md) uniquely.

## ↑ Ancestors (13)

1. [Grounded hemisphere](../grounded-hemisphere.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

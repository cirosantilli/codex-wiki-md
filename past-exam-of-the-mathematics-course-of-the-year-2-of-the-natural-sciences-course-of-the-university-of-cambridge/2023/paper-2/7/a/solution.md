<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the stated square side length $2a$, the volume is $4a^2h$ and the uniform [mass density](../../../../../density.md) is $\rho_1=m_1/(4a^2h)$. Direct integration about its central vertical axis gives the [moment of inertia of a uniform square plate](../../../../../moment-of-inertia-of-a-uniform-square-plate.md):

$$
I_1=\rho_1h\int_{-a}^a\int_{-a}^a(x^2+y^2)\,dx\,dy
=\rho_1h\frac{8a^4}{3}
=\boxed{\frac23m_1a^2}.
$$

Thus the PDF's coefficient $1/6$ is inconsistent with its stated side length. The coefficient $1/6$ would apply to a square of side $a$.

For the disc, use [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md) and $m_2=\rho_2\pi a^2h$:

$$
I_2=\rho_2h\int_0^{2\pi}\int_0^a r^2r\,dr\,d\theta
=\frac{\pi\rho_2ha^4}{2}=\boxed{\frac12m_2a^2}.
$$

For the sphere, use [spherical coordinates](../../../../../spherical-coordinate-system.md) and $m_3=4\pi\rho_3a^3/3$:

$$
I_3=\rho_3\int_0^a r^4dr\int_0^\pi\sin^3\theta\,d\theta\int_0^{2\pi}d\phi
=\frac{8\pi\rho_3a^5}{15}=\boxed{\frac25m_3a^2}.
$$

These agree with the [moment of inertia of a uniform disc](../../../../../moment-of-inertia-of-a-uniform-disc.md) and the [moment of inertia of a uniform solid sphere](../../../../../moment-of-inertia-of-a-uniform-solid-sphere.md). The square's thickness does not enter its axial [moment of inertia](../../../../../moment-of-inertia.md) once the mass is fixed.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [7](../../7.md)
3. [Paper 2](../../../paper-2-split.md)
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

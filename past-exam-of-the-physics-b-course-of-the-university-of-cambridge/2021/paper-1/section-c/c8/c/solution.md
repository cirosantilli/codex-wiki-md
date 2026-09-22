<h1 id="section-c/c8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Consider a long uniform length $\ell$ of a [coaxial cylindrical capacitor](../../../../../../coaxial-cylindrical-capacitor.md), with permittivity $\epsilon_0\epsilon_r$ and inner-cylinder charge per unit length $\lambda$. A cylindrical [Gaussian surface](../../../../../../gaussian-surface.md) gives

$$
D_r=\frac{\lambda}{2\pi r},\qquad
E_r=\frac{\lambda}{2\pi\epsilon_0\epsilon_r r},\qquad a<r<b.
$$

The [electric potential difference](../../../../../../electric-potential-difference.md) is

$$
V=\int_a^bE_r\,dr=\frac{\lambda\ln(b/a)}{2\pi\epsilon_0\epsilon_r}.
$$

Thus its [capacitance](../../../../../../capacitance.md) per unit length is $c(\epsilon_r)=2\pi\epsilon_0\epsilon_r/\ln(b/a)$.

In the [partially filled coaxial capacitor](../../../../../../partially-filled-coaxial-capacitor.md), the vacuum section of length $L-x$ and the dielectric section of length $x$ share the same two conductors and hence the same [electric potential difference](../../../../../../electric-potential-difference.md). They are electrically in parallel, not in series. The radial [electric field](../../../../../../electric-field-split.md) is tangent to the axial dielectric interface, consistent with the boundary condition in part (b). Adding their charges gives

$$
\boxed{C=c(1)(L-x)+c(\epsilon)x
=\frac{2\pi\epsilon_0}{\ln(b/a)}[L-x+\epsilon x].}
$$

This is the leading long-capacitor expression, neglecting end and interface-fringing corrections. The stated $x\gg b$ supports a long filled section; treating the other section as uniform also requires it to be well away from the end regions when those corrections matter.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [C8](../../c8.md)
3. [Section C](../../../section-c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)

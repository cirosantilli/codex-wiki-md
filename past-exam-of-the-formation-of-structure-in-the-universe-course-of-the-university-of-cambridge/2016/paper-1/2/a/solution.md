<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [binding energy of a truncated singular isothermal sphere](../../../../../binding-energy-of-a-truncated-singular-isothermal-sphere.md), build the mass distribution from concentric shells. Its [enclosed mass](../../../../../enclosed-mass.md) and mass element are

$$
M(r)=\int_0^r4\pi s^2\rho(s)\,\mathrm ds
=\frac{2k}{G}r,\qquad
\mathrm dM=\frac{2k}{G}\,\mathrm dr,
\qquad M_0=\frac{2kr_0}{G}.
$$

The interaction of a newly added shell with the interior contributes $-GM(r)\,\mathrm dM/r$. Counting each pair once,

$$
W=-\int_0^{r_0}\frac{GM(r)}r\,\mathrm dM(r)
=-\frac{4k^2}{G}\int_0^{r_0}\mathrm dr
=-\frac{4k^2r_0}{G}.
$$

Eliminating $k$ gives

$$
\boxed{W=-\frac{GM_0^2}{r_0}.}
$$

The central density is singular, but the mass and this energy integral are finite. The result assumes the stated truncation and no additional gravitating component.

The [gravitational potential of a truncated singular isothermal sphere](../../../../../gravitational-potential-of-a-truncated-singular-isothermal-sphere.md) is a separate quantity from this shell-assembly energy allocation. With zero potential at infinity, both interior and exterior shells contribute:

$$
\Phi_{\rm grav}(r)
=-G\left[\frac{M(r)}r+\int_r^{r_0}\frac{\mathrm dM(s)}s\right]
=-2k\left[1+\ln\frac{r_0}r\right],\quad0<r\leq r_0.
$$

It matches $-GM_0/r_0=-2k$ at the edge. The equivalent total energy is $W=\tfrac12\int\rho\Phi_{\rm grav}\,\mathrm dV$; the half prevents double counting. By contrast, $\int\rho[-\Phi_{\rm grav}]\,\mathrm dV$ counts the escape work of test parcels in a fixed potential and equals $-2W$. Confusing these quantities would change a local feedback threshold.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the formation of Structure in the Universe course of the University of Cambridge](../../../../split.md)
6. [Formation of Structure in the Universe course of the University of Cambridge](../../../../../formation-of-structure-in-the-universe-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)

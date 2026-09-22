<h1 id="1/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

To hold sphere 2 fixed against the incident angular velocity from part ii, its applied couple must generate the bare rotation

$$
\widetilde{\boldsymbol\Omega}_2
=\frac{\mathbf G_2}{8\pi\mu a^3}
=-\frac{a^3}{2R^3}\left[
3\frac{(\boldsymbol\Omega\cdot\mathbf R)\mathbf R}{R^2}
-\boldsymbol\Omega
\right].
$$

The resulting [rotlet](../../../../../../../rotlet.md) advects the force-free sphere 1. Since the field is harmonic, [Faxén's first law](../../../../../../../faxen-s-first-law.md) gives

$$
\mathbf U_1
=a^3\frac{\widetilde{\boldsymbol\Omega}_2\times(-\mathbf R)}{R^3}
=\boxed{-\frac{a^6}{2R^6}\boldsymbol\Omega\times\mathbf R}.
$$

The returned rotlet has velocity $O(\Omega a^6/R^5)$ and rate of strain $O(\Omega a^6/R^6)$ at sphere 1. That strain induces a [stresslet](../../../../../../../force-dipole-flow.md) of strength $O(\mu\Omega a^9/R^6)$, whose velocity at sphere 2 is $O(\Omega a^9/R^8)$. This [method of reflections for Stokes flow](../../../../../../../method-of-reflections-for-stokes-flow.md) gives the stated order of the next correction to $\mathbf U_2$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 329](../../../../paper-329-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

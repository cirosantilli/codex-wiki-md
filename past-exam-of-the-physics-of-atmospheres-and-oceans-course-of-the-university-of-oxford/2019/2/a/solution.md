<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $S$ as the integrated line [mass absorption coefficient](../../../../mass-absorption-coefficient.md), and $q$ as the absorber [mass fraction](../../../../mass-fraction.md), assumed constant; for a pure absorbing gas set $q=1$. All spectral intervals below use the paper's wavenumber coordinate. The normalized [Lorentz line shape](../../../../lorentz-line-shape.md) is

$$
\kappa_\nu(p)=\frac{S}{\pi}\frac{\Delta(p)}{(\nu-\nu_0)^2+\Delta(p)^2},\qquad
\boxed{\kappa_{\nu_0}(p)=\frac{S}{\pi\Delta(p)}.}
$$

If instead an absorption coefficient per length is wanted, multiply by absorber [density](../../../../density.md). Neglecting temperature dependence, [pressure broadening](../../../../pressure-broadening.md) gives $\Delta(p)=\Delta_s p/p_s$. In the line wings, with $d=|\nu-\nu_0|\gg\Delta(p)$,

$$
\kappa_\nu\simeq\frac{S\Delta_s p}{\pi p_s d^2},\qquad
\tau_\nu(p)\simeq\frac{qS\Delta_s p^2}{2\pi gp_s d^2}.
$$

Define the line-opacity parameter and characteristic wavenumber width

$$
C=\frac{qSp_s}{2\pi g\Delta_s},\qquad w=\Delta_s\sqrt C.
$$

At an emitting level $\tau_\nu\sim1$, the wing estimate implies $d/\Delta(p)\sim\sqrt C$. Thus the [strong-line limit](../../../../strong-line-limit.md) relevant to outgoing radiation is

$$
\boxed{C\gg1,\quad\text{equivalently }qSp_s/(g\Delta_s)\gg1\text{ up to fixed factors}.}
$$

It ensures that the opaque-to-transparent transition lies in the Lorentz wings, rather than the narrow central core, and the characteristic absorption width is much larger than $\Delta_s$. At a grazing ray angle the criterion is even easier to satisfy because of the larger [optical depth](../../../../optical-depth.md). This is a criterion for the radiatively important wings, not a claim that collision broadening remains physical at arbitrarily small [pressure](../../../../pressure-split.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

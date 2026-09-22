<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the stated gravity-dominated approximation, neglect the pressure force in the radial momentum equation. A steady outward [stellar wind](../../../../../stellar-wind.md) then obeys

$$
v\frac{dv}{dr}=-\frac{GM_*}{r^2},\qquad
\frac{v^2}{2}-\frac{GM_*}{r}=C.
$$

At $R_e=R_{\rm esc}$, the [escape velocity](../../../../../escape-velocity.md) is $v_e=\sqrt{2GM_*/R_e}$, so $C=0$. The [ballistic marginal-escape stellar wind](../../../../../ballistic-marginal-escape-stellar-wind.md) has

$$
\boxed{v(r)=\sqrt{\frac{2GM_*}{r}}
=v_e\left(\frac r{R_e}\right)^{-1/2}.}
$$

The outward flow decelerates and approaches zero speed at infinity; it is exactly at the escape threshold in this pressure-negligible model. An initial speed above that threshold gives a nonzero asymptotic speed.

Adiabaticity alone would instead conserve the full [Bernoulli equation](../../../../../bernoulli-equation.md) $v^2/2+h-GM_*/r=B$. If finite pressure is retained and $v_e$ equals the mechanical escape speed, then $B=h_e$, not zero. With $p=K\rho^\gamma$ and [conservation of mass](../../../../../mass-conservation.md), the more general implicit solution is

$$
\frac{v^2}{2}-\frac{GM_*}{r}
+h_e\left(\frac{R_e^2v_e}{r^2v}\right)^{\gamma-1}=h_e.
$$

It needs $h_e$ and $\gamma$ in addition to the escape-speed datum. The boxed explicit power law is the leading gravity-dominated result, not an exact solution for an arbitrary warm adiabatic wind.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
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

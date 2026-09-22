<h1 id="10/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Use the supplied planet [mass](../../../../mass.md) $5.9\times10^{24}\,\mathrm{kg}$, $G=6.67430\times10^{-11}\,\mathrm{m^3\,kg^{-1}\,s^{-2}}$, and adopt mean Earth radius $R_E=6371\,\mathrm{km}$. For a [geostationary orbit](../../../../geostationary-orbit.md), use one [sidereal day](../../../../sidereal-day.md), $T\simeq86164\,\mathrm s$. The adopted radius and rotation period follow NASA's fact sheet.[Bulk parameters: volumetric mean radius6371.000km; orbital parameters: sidereal rotation period23.9345hours](../../../../earth-fact-sheet-by-national-aeronautics-and-space-administration.md)

$$
r_0=R_E+300\,\mathrm{km}=6.671\times10^6\,\mathrm m,\qquad r_1=\left(\frac{\mu T^2}{4\pi^2}\right)^{1/3}\simeq4.1994\times10^7\,\mathrm m.
$$

The slightly smaller radius than the usual terrestrial value follows from using the question's smaller Earth [mass](../../../../mass.md). For coplanar prograde orbits, the preceding formulas give

$$
\Delta v_1\simeq2.410\,\mathrm{km\,s^{-1}},\qquad\Delta v_2\simeq1.459\,\mathrm{km\,s^{-1}},\qquad\boxed{\Delta v_H\simeq3.869\,\mathrm{km\,s^{-1}}.}
$$

The escape transfer has $a\to\infty$, so its first tangential burn reaches the local [escape speed](../../../../escape-velocity.md) $\sqrt{2\mu/r_0}$. No final circularization at infinity is needed:

$$
\boxed{\Delta v_{\mathrm{escape}}=(\sqrt2-1)\sqrt{\frac\mu{r_0}}\simeq3.182\,\mathrm{km\,s^{-1}}.}
$$

Thus the geostationary transfer requires about $0.687\,\mathrm{km\,s^{-1}}$ more total impulse, or about 22 percent more, despite leaving the spacecraft gravitationally bound. Reaching the outer radius and circularizing there are separate requirements. Changing the starting orbit's inclination would add a plane-change cost absent from this calculation.

## ↑ Ancestors (12)

1. [V](../v.md)
2. [10](../../10.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the physics 1 paper of the University of Oxford](../../../split.md)
5. [Physics 1 paper of the University of Oxford](../../../../physics-1-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

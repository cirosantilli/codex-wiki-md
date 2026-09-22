<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the shallower initial density profile,

$$
M_0(r)=\frac{k'}G r^2,\qquad
M_0=\frac{k'r_0^2}{G}.
$$

Including outer shells, the initial [gravitational potential](../../../../../newtonian-potential-of-a-point-mass.md) is

$$
\Phi_{\rm grav}(r)
=-G\left[\frac{M_0(r)}r+\int_r^{r_0}\frac{\mathrm dM_0(s)}s\right]
=-k'(2r_0-r).
$$

Its central value is finite. With the same remaining-gas escape criterion and fixed-potential approximation as above,

$$
\boxed{r_{\rm quench}(t)
=2r_0-\frac{q}{k'}(e^{\nu t}-1).}
$$

This front is inside the [galaxy](../../../../../galaxy-split.md) only when $k'r_0\leq Q(t)\leq2k'r_0$. Thus

$$
t_{\rm start}=\nu^{-1}\ln\left(1+\frac{k'r_0}{q}\right),\qquad
t_{\rm all}=\nu^{-1}\ln\left(1+\frac{2k'r_0}{q}\right).
$$

Quenching still moves **from the outside inward**, but now reaches the centre in a finite time. The contrast with the $r^{-2}$ escape model is the finite central potential, not a reversed gravitational force.

Under the alternative [shell-energy quenching prescription](../../../../../shell-energy-quenching-prescription.md), the conclusion is different:

$$
B_{\rm shell}(r)=\frac{GM_0(r)}r=k'r,\qquad
\boxed{r_{\rm quench}^{\rm shell}(t)=\frac q{k'}(e^{\nu t}-1).}
$$

Here the quenched region is inside the front and grows **from the centre outward**, unlike the simultaneous quenching of the isothermal shell-allocation model. Its edge reaches $r_0$ at $\nu^{-1}\ln(1+k'r_0/q)$. This change of direction is a consequence of the chosen local energy model: $GM(r)/r$ increases with radius for this profile, whereas the true binding potential including all outer shells always becomes shallower outward. The source does not identify which local allocation it intends; keeping the conventions explicit resolves the different conditional predictions without discarding the exterior-shell potential.

## ↑ Ancestors (14)

1. [C](../c.md)
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

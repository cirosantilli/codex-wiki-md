<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $t_0$ be the initial epoch, let $r(t)$ be the physical radius of the outer matter shell, and put $r(t_0)=r_0$. The background [Einstein-de Sitter universe](../../../../einstein-de-sitter-universe.md) has [critical density](../../../../critical-density.md) $\rho_b=3H_i^2/(8\pi G)$ at that epoch. Its mass inside $r_0$ is $M_b=M-\delta M$, where $M$ is the actual conserved mass. Hence the background [Friedmann equation](../../../../friedmann-equations.md) implies

$$
H_i^2=\frac{2G(M-\delta M)}{r_0^3},\qquad
\dot r_0^2=H_i^2r_0^2=\frac{2G(M-\delta M)}{r_0}.
$$

For [spherical collapse](../../../../spherical-collapse-model.md) of pressureless matter, with no [shell crossing](../../../../shell-crossing.md), the [shell theorem](../../../../spherical-shell-theorem.md) gives $\ddot r=-GM/r^2$. Its [conservation of energy](../../../../conservation-of-energy.md) first integral is

$$
\frac12\dot r^2-\frac{GM}{r}
=\frac12\dot r_0^2-\frac{GM}{r_0}
=-\frac{G\delta M}{r_0}.
$$

Consequently

$$
\dot r^2=\frac Ar-B,\qquad
\boxed{A=2GM,\qquad B=\frac{2G\delta M}{r_0}.}
$$

For $\delta M>0$, the initially expanding branch reaches [cosmological turnaround](../../../../cosmological-turnaround.md) at $r_{\rm ta}=A/B=Mr_0/\delta M$. Since $dt=dr/\dot r$ on that branch, the elapsed [cosmic time](../../../../cosmic-time.md) is

$$
\boxed{\tau=t_{\rm ta}-t_0
=\int_{r_0}^{A/B}\sqrt{\frac r{A-Br}}\,dr.}
$$

This is [spherical turnaround from an unperturbed Hubble velocity](../../../../spherical-turnaround-from-an-unperturbed-hubble-velocity.md). The integral measures the comoving matter observers' time interval in the pressureless model. The integration variable is the physical radius, not the radius divided by the background [scale factor](../../../../scale-factor-cosmology.md). If an absolute [cosmic time](../../../../cosmic-time.md) is wanted, add $t_0$ to the displayed interval.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the general relativity course of the University of Oxford](../../../split.md)
5. [General relativity course of the University of Oxford](../../../../general-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

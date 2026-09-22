<h1 id="section-b/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use [plane wave](../../../../../plane-wave.md) perturbations proportional to $e^{i(k_xx+k_zz-\omega t)}$, with amplitudes $\widehat u,\widehat w,\widehat\pi,\widehat\varrho$. The linear equations become

$$
k_x\widehat u+k_z\widehat w=0,\qquad
\omega\rho_0\widehat u=k_x\widehat\pi,\qquad
-i\omega\rho_0\widehat w=-ik_z\widehat\pi-g\widehat\varrho,\qquad
-i\omega\widehat\varrho=-\rho'_0\widehat w.
$$

To eliminate [pressure](../../../../../pressure-split.md) without dividing by $k_x$, multiply the vertical momentum equation by $k_x$ and subtract $k_z$ times the horizontal momentum equation:

$$
-i\omega\rho_0(k_x\widehat w-k_z\widehat u)=-gk_x\widehat\varrho.
$$

Use [incompressible flow](../../../../../incompressible-flow.md) and the equation for [mass density](../../../../../density.md) to obtain $\omega^2\rho_0(k_x^2+k_z^2)\widehat w=-g\rho'_0k_x^2\widehat w$. Hence, for a nontrivial [internal gravity wave](../../../../../internal-wave.md),

$$
\boxed{\omega^2=N^2\frac{k_x^2}{k_x^2+k_z^2},\qquad
N^2=-\frac{g\rho'_0}{\rho_0}.}
$$

For stable [density stratification](../../../../../density-stratification.md), $\rho'_0<0$ and $N=\sqrt{-g\rho'_0/\rho_0}$ is the [buoyancy frequency](../../../../../buoyancy-frequency.md). Then $0\le\omega^2\le N^2$ and the [normal modes](../../../../../normal-mode.md) oscillate rather than grow. For $\rho'_0>0$, a mode with $k_x\ne0$ has $\omega^2<0$ and grows exponentially: denser fluid lies above lighter fluid. Uniform density, $\rho'_0=0$, is marginal for this restoring mechanism.

The case $k_x=0$, $k_z\ne0$, has zero [frequency](../../../../../frequency.md) in the displayed relation. [Incompressible flow](../../../../../incompressible-flow.md) then requires $\widehat w=0$, so it is a degenerate non-propagating case rather than a finite-frequency vertical oscillation. These equations concern the incompressible model of part (b); its $N^2$ does not contain the adiabatic compression correction needed in part (a).

## ↑ Ancestors (14)

1. [C](../c.md)
2. [4](../../4.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
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

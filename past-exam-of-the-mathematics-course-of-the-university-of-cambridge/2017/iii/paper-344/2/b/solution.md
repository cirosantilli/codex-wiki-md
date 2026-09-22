<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [dynamical scaling of binary-fluid coarsening](../../../../../../dynamical-scaling-of-binary-fluid-coarsening.md) assumes a statistically self-similar bicontinuous morphology with one growing length $L$, thin interfaces, curvature of order $1/L$, and typical fluid speed of order $\dot L$. Inertial acceleration then scales as $\ddot L$ and $\dot L^2/L$, viscous force density as $\eta\dot L/L^2$, and capillary force density as $\sigma/L^2$. The [pressure](../../../../../../pressure.md) is eliminated or estimated together with the interfacial force. The numerical coefficients summarize geometry and projected force directions; this is a scaling closure, not a spatially exact momentum equation.

The approximation further neglects diffusive growth relative to advective growth, assumes fixed volume fraction and material parameters, no external forcing, and no additional relevant macroscopic length. A finite initial domain size, interface width or finite container would introduce further ratios outside the asymptotic scaling regime. Velocity [gradients](../../../../../../gradient.md) need not stay on the domain scale in a genuinely multiscale turbulent flow, so this single-length argument is not a proof for every hydrodynamic morphology.

With $[\rho]=\mathrm{M\,L^{-3}}$, $[\eta]=\mathrm{M\,L^{-1}\,T^{-1}}$ and $[\sigma]=\mathrm{M\,T^{-2}}$, [dimensional analysis](../../../../../../dimensional-analysis.md) gives the unique scales

$$
L_0=\frac{\eta^2}{\rho\sigma},\qquad t_0=\frac{\eta^3}{\rho\sigma^2},\qquad \frac{L_0}{t_0}=\frac\sigma\eta.
$$

Thus, within the stated asymptotic single-scale hypothesis, the [hydrodynamic coarsening crossover scales](../../../../../../hydrodynamic-coarsening-crossover-scales.md) give $L=L_0f(u)$, $u=t/t_0$. All four force-density terms have the same dimensional prefactor $\rho^2\sigma^3/\eta^4$. Dividing by it yields

$$
\boxed{\alpha f''+\beta\frac{f'^2}{f}=\gamma\frac{f'}{f^2}+\frac\delta{f^2}.}
$$

Primes denote $d/du$. The PDF includes $\eta\gamma\dot L/L^2$; the TeX drops $\eta$. The PDF expression is dimensionally consistent. For a positive growth branch, a resisting viscous term and a driving capillary term have opposite signed coefficients; one may set $\gamma=-c_v<0$, $\delta=c_s>0$. The question calls these coefficients order one, not positive. Treating every term on the printed right-hand side as positive would lose the viscous-capillary balance.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

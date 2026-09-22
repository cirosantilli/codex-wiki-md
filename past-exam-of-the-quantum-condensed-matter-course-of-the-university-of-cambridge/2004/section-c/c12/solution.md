<h1 id="section-c/c12/solution">Solution</h1>

↑ **Parent:** [C12](../c12.md)

Put $z=e^{\beta\mu}$, with $\beta=1/(k_BT)$. For a single quantum state of [energy](../../../../energy-split.md) $\epsilon$, dilute [Maxwell–Boltzmann statistics](../../../../maxwell-boltzmann-statistics.md) gives $\ln\Xi_\epsilon\simeq ze^{-\beta\epsilon}$. For bosons this is the leading expansion of $-\ln(1-ze^{-\beta\epsilon})$; the occupation must be small for that expansion. Thus the [grand potential](../../../../grand-potential.md) is

$$
\boxed{\Phi(\epsilon)=-k_BT\ln\Xi_\epsilon\simeq-k_BT e^{-\beta(\epsilon-\mu)}.}
$$

With the ground-state [energy](../../../../energy-split.md) set to zero, a dilute classical gas requires $e^{\beta\mu}\ll1$, giving negative $\mu$. This sign is relative to the chosen [energy](../../../../energy-split.md) zero. For an ideal Bose gas, $\mu$ approaches the ground [energy](../../../../energy-split.md) from below at condensation, so it approaches zero with this convention.

The printed degeneracy formula requires $n_x,n_y,n_z=0,1,2,\ldots$, rather than strictly positive integers. With zero-point [energy](../../../../energy-split.md) omitted these are the appropriate oscillator quantum numbers. The [stars and bars](../../../../stars-and-bars-combinatorics.md) count of three nonnegative integers summing to $n$ gives

$$
\boxed{d_n=\binom{n+2}{2}=\frac{(n+2)!}{n!\,2!}.}
$$

There is one ground state at $n=0$. If the integers were strictly positive, the count would instead be $\binom{n-1}{2}$ for $n\geq3$, inconsistent with both the printed formula and its [energy](../../../../energy-split.md) reference.

For large $n$, $d_n\simeq n^2/2$. Consecutive [energy](../../../../energy-split.md) shells are separated by $\hbar\omega$, giving the continuum [density of states](../../../../density-of-states.md)

$$
\boxed{g(E)\simeq\frac{n^2}{2\hbar\omega}=\frac{E^2}{2(\hbar\omega)^3}.}
$$

Use this when $k_BT\gg\hbar\omega$, and integrate the single-state grand potential over [energy](../../../../energy-split.md):

$$
\Phi_{\rm tot}\simeq-\frac{k_BT e^{\beta\mu}}{2(\hbar\omega)^3}\int_0^\infty E^2e^{-\beta E}dE=-\frac{(k_BT)^4}{(\hbar\omega)^3}e^{\beta\mu},
$$

because the integral is $2/\beta^3$. Particle number follows by differentiating at fixed [temperature](../../../../temperature-split.md) and trap [frequency](../../../../frequency.md):

$$
N=-\frac{\partial\Phi}{\partial\mu}=\left(\frac{k_BT}{\hbar\omega}\right)^3e^{\beta\mu},\qquad\boxed{\mu=k_BT\ln\left[N\left(\frac{\hbar\omega}{k_BT}\right)^3\right].}
$$

These are the high-temperature expressions for the [classical grand potential in a harmonic trap](../../../../classical-grand-potential-in-a-harmonic-trap.md).

Extrapolating to $\mu=0$ gives the requested transition scale

$$
\boxed{T_c\sim\frac{\hbar\omega}{k_B}N^{1/3}.}
$$

It is an order-one estimate because Maxwell-Boltzmann occupations cease to be accurate near condensation. The [Bose-Einstein distribution](../../../../bose-einstein-distribution.md) gives the more precise ideal-trap result $N_{\rm ex}^{\max}=\zeta(3)(k_BT/\hbar\omega)^3$, and hence $T_c=(\hbar\omega/k_B)[N/\zeta(3)]^{1/3}$, about $0.94$ times the estimate. Excess particles populate the ground state after the excited-state capacity saturates: [Bose condensation in a three-dimensional harmonic trap](../../../../bose-condensation-in-a-three-dimensional-harmonic-trap.md).

The [observation of Bose-Einstein condensation in rubidium in 1995](../../../../observation-of-bose-einstein-condensation-in-rubidium-in-1995.md) implemented laser precooling followed by radio-frequency evaporation from a magnetic trap. Imaging the released cloud revealed a narrow anisotropic component within a broader thermal population. This provides an experimental connection to the population-counting argument; the measured expansion also reflects interactions and imaging resolution, not just the ideal-trap [density of states](../../../../density-of-states.md).[1995, pp. 198–201, Figs. 1–4](../../../../observation-of-bose-einstein-condensation-in-a-dilute-atomic-vapor-by-m-h-anderson-and-others.md)

## ↑ Ancestors (13)

1. [C12](../c12.md)
2. [Section C](../../section-c.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../split.md)
5. [Quantum Condensed Matter course of the University of Cambridge](../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)

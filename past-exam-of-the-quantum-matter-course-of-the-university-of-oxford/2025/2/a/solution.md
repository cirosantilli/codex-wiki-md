<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Measure single-particle [energy](../../../../energy-split.md) from the [quantum harmonic oscillator](../../../../quantum-harmonic-oscillator-split.md) [ground state](../../../../ground-state.md) [energy](../../../../energy-split.md) $\hbar\omega$, and write $\widetilde\mu=\mu_{\mathrm{physical}}-\hbar\omega\leq0$. The [Bose-Einstein distribution](../../../../bose-einstein-distribution.md) and the supplied [density of states](../../../../density-of-states.md) give

$$
N_{\mathrm{ex}}(T,\widetilde\mu)=\int_0^\infty\frac{E\,dE}{(\hbar\omega)^2[e^{(E-\widetilde\mu)/(k_BT)}-1]}.
$$

This excited-state population increases with the [chemical potential](../../../../chemical-potential-split.md) and has the finite saturation value

$$
N_{\mathrm{ex}}^{\max}(T)=\left(\frac{k_BT}{\hbar\omega}\right)^2\int_0^\infty\frac{u\,du}{e^u-1}
=\frac{\pi^2}{6}\left(\frac{k_BT}{\hbar\omega}\right)^2.
$$

Any additional particles must occupy the [ground state](../../../../ground-state.md): this is [two-dimensional harmonic-trap Bose condensation](../../../../two-dimensional-harmonic-trap-bose-condensation.md). The [critical temperature](../../../../critical-temperature.md) and the [condensate fraction](../../../../condensate-fraction.md) are therefore

$$
\boxed{N\omega^2=\frac{\pi^2}{6}\left(\frac{k_BT_c}{\hbar}\right)^2,\qquad
k_BT_c=\frac{\hbar\omega\sqrt{6N}}\pi,\qquad
N_0(T)=\begin{cases}N[1-(T/T_c)^2],&T\leq T_c,\\0,&T>T_c.\end{cases}}
$$

Here $N$ is the total [particle number](../../../../particle-number.md), the integral of the inhomogeneous [number density](../../../../number-density.md) over the trap; there is no fixed uniform area in which $N$ itself is a [number density](../../../../number-density.md). Equivalently $N\kappa=\pi^2m(k_BT_c)^2/(6\hbar^2)$ relates the trap population to the [critical temperature](../../../../critical-temperature.md). Harmonic confinement changes the low-[energy](../../../../energy-split.md) [density of states](../../../../density-of-states.md) and permits this saturation in two spatial dimensions.

These formulas are leading large-$N$ results with $k_BT_c\gg\hbar\omega$. A sharp transition belongs to the trapped-gas [thermodynamic limit](../../../../thermodynamic-limit.md) $N\to\infty$, $\omega\to0$ at fixed $N\omega^2$; a finite trap has [finite-size rounding](../../../../finite-size-rounding.md). In particular, finite $N_0$ requires $\widetilde\mu=-k_BT\log(1+1/N_0)<0$, approaching zero in the condensation limit.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the quantum matter course of the University of Oxford](../../../split.md)
5. [Quantum matter course of the University of Oxford](../../../../quantum-matter-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

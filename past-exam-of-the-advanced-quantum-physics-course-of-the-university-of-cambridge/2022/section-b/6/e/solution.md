<h1 id="section-b/6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The thermal oscillator occupation is the [Bose-Einstein distribution](../../../../../bose-einstein-distribution.md). With the rate notation $\Gamma_{\eta\sigma}$ for a transition from $\sigma$ to $\eta$, the [master equation](../../../../../master-equation.md) for the up population is

$$
\frac{dp_\uparrow}{dt}=\Gamma_{\uparrow\downarrow}p_\downarrow
-\Gamma_{\downarrow\uparrow}p_\uparrow
=\Gamma_0\left[n_\Omega p_\downarrow-(n_\Omega+1)p_\uparrow\right].
$$

At [thermal equilibrium](../../../../../thermal-equilibrium-split.md), assuming $\Gamma_0>0$, vanishing time derivative is [detailed balance](../../../../../detailed-balance.md) between the two spin states. Hence

$$
\frac{p_\uparrow}{p_\downarrow}=\frac{n_\Omega}{n_\Omega+1}
=\frac{1/(e^{\beta\hbar\Omega}-1)}{e^{\beta\hbar\Omega}/(e^{\beta\hbar\Omega}-1)}
=e^{-\beta\hbar\Omega},
$$

or

$$
\boxed{p_\uparrow=e^{-\beta\hbar\Omega}p_\downarrow.}
$$

Together with normalization, this gives $p_\uparrow=1/(1+e^{\beta\hbar\Omega})$ and $p_\downarrow=e^{\beta\hbar\Omega}/(1+e^{\beta\hbar\Omega})$, the [Boltzmann distribution](../../../../../boltzmann-distribution.md) for the [energy eigenvalues](../../../../../energy-eigenvalue-split.md) $\pm\hbar\Omega/2$. At zero temperature, absorption vanishes and emission relaxes the spin into its down ground state.

The nonzero-rate condition is necessary: if $\lambda=0$ or $g(\Omega)=0$, both rates vanish, so every initial pair of populations is stationary within this approximation. In that case stationarity alone cannot imply a thermal distribution. The equilibrium conclusion therefore presumes coupling to resonant oscillator modes.

## ↑ Ancestors (14)

1. [E](../e.md)
2. [6](../../6.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the advanced quantum physics course of the University of Cambridge](../../../../split.md)
6. [Advanced Quantum Physics course of the University of Cambridge](../../../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)

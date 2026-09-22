# Gaussian variational bounds for a quartic oscillator

↑ **Parent:** [Variational method](variational-method.md)

For $H=p^2/(2m)+kx^4$ with $k>0$, the normalized even trial [wavefunction](wave-function-split.md) $f_\alpha=(\alpha/\pi)^{1/4}e^{-\alpha x^2/2}$ has [Rayleigh quotient](rayleigh-quotient.md)

$$
\mathcal E_0(\alpha)=\frac{\hbar^2\alpha}{4m}+\frac{3k}{4\alpha^2}.
$$

The [Gaussian moment recurrence](gaussian-moment-recurrence.md) gives the potential term, and [integration by parts](integration-by-parts.md) gives the kinetic term. Its minimum is at $\alpha^3=6mk/\hbar^2$, proving the displayed upper bound by the [Rayleigh-Ritz variational principle](rayleigh-ritz-variational-principle.md).

An odd trial family $g_\beta=(4\beta^3/\pi)^{1/4}x e^{-\beta x^2/2}$ is orthogonal to the exact even [ground state](ground-state.md). The [Sturm oscillation theorem](sturm-oscillation-theorem.md) identifies the lowest odd state as the first excited state, so minimizing within this family bounds $E_1$:

$$
\mathcal E_1(\beta)=\frac{3\hbar^2\beta}{4m}+\frac{15k}{4\beta^2},\quad
\beta_*^3=\frac{10mk}{\hbar^2},\quad
E_1\leq\frac{9\hbar^2}{8m}\left(\frac{10mk}{\hbar^2}\right)^{1/3}.
$$

Orthogonality to an approximate ground trial alone would not justify this excited-state bound; odd parity ensures orthogonality to the exact ground state. Both bounds exhibit the characteristic quartic-oscillator [energy](energy-split.md) scale $(\hbar^4k/m^2)^{1/3}$.

**Table of contents**

- [Gaussian trial for a quadratic-plus-quartic oscillator](gaussian-trial-for-a-quadratic-plus-quartic-oscillator.md)

## ↑ Ancestors (5)

1. [Variational method](variational-method.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2021/section-a/3/solution.md)

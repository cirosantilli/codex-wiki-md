# Bose condensation in a three-dimensional harmonic trap

↑ **Parent:** [Dilute-gas Bose-Einstein condensation](dilute-gas-bose-einstein-condensation.md)

Consider $N$ noninteracting [bosons](boson.md) in one internal [quantum state](quantum-state.md), at [thermal equilibrium](thermal-equilibrium-split.md) in the three-dimensional [harmonic oscillator](simple-harmonic-motion.md) potential

$$
V(\mathbf r)=\frac m2(\omega_x^2x^2+\omega_y^2y^2+\omega_z^2z^2),\qquad
\bar\omega=(\omega_x\omega_y\omega_z)^{1/3}.
$$

Here $m$ is the [mass](mass.md), the positive $\omega_i$ are [angular frequencies](angular-frequency.md), and $\bar\omega$ is their [geometric mean](geometric-mean.md). Measure the one-particle [energy](energy-split.md) $\epsilon$ and [chemical potential](chemical-potential-split.md) $\mu$ from the [ground-state energy](ground-state-energy.md). The [quantum harmonic oscillator](quantum-harmonic-oscillator-split.md) levels then have $\epsilon=\hbar(\omega_x n_x+\omega_y n_y+\omega_z n_z)$ with nonnegative integer $n_i$ and reduced [Planck constant](planck-constant.md) $\hbar=h/(2\pi)$.

When $\epsilon\gg\hbar\omega_i$, counting [lattice points](lattice-point.md) can be approximated by the volume of a [tetrahedron](tetrahedron.md) in the positive octant of $(n_x,n_y,n_z)$:

$$
\mathcal N(\epsilon)\simeq\frac{\epsilon^3}{6\hbar^3\omega_x\omega_y\omega_z},\qquad
g(\epsilon)=\frac{d\mathcal N}{d\epsilon}\simeq\frac{\epsilon^2}{2(\hbar\bar\omega)^3}.
$$

This is a [density of states](density-of-states.md), with units of inverse [energy](energy-split.md). The factor $1/6$ is the unit tetrahedron volume; differentiating produces the factor $1/2$. Treat the single [ground state](ground-state.md) separately: its macroscopic population would be lost by replacing every level with a smooth [density of states](density-of-states.md).

For $k_BT\gg\hbar\omega_i$, integrate the [Bose-Einstein distribution](bose-einstein-distribution.md) over excited [energy eigenstates](energy-eigenstate.md). As $\mu$ approaches zero from below, their maximum population is

$$
N_{\rm ex}^{\rm sat}(T)=\int_0^\infty\frac{g(\epsilon)\,d\epsilon}{e^{\epsilon/(k_BT)}-1}
=\zeta(3)\left(\frac{k_BT}{\hbar\bar\omega}\right)^3.
$$

Here $k_B$ is the [Boltzmann constant](boltzmann-constant.md) and $\zeta$ the [Riemann zeta function](riemann-zeta-function.md). A short proof uses $1/(e^x-1)=\sum_{\ell\ge1}e^{-\ell x}$ and $\int_0^\infty x^2e^{-\ell x}dx=2/\ell^3$. The nonnegative terms permit exchanging [summation](summation.md) and [integration](integral-split.md) by [Tonelli's theorem](tonelli-theorem.md), giving $\int_0^\infty x^2/(e^x-1)dx=2\zeta(3)$. Near zero the integrand is proportional to $x$, so its integral converges. That finite excited-state capacity is the mechanism of [Bose-Einstein condensation](bose-einstein-condensation.md).

Set $N_{\rm ex}^{\rm sat}(T_c)=N$. Particle conservation gives, to this continuum accuracy,

$$
k_BT_c=\hbar\bar\omega\left(\frac{N}{\zeta(3)}\right)^{1/3},\qquad
\frac{N_0}{N}=1-\left(\frac{T}{T_c}\right)^3\quad(0\le T\le T_c).
$$

Above $T_c$, the macroscopic [condensate fraction](condensate-fraction.md) is zero and the [chemical potential](chemical-potential-split.md) adjusts below zero. This cubic power belongs to a three-dimensional harmonic trap; it is not the homogeneous three-dimensional [ideal gas](ideal-gas-split.md) exponent. For $N=10^5$, $\bar\omega/(2\pi)=100\,\mathrm{Hz}$ and $\zeta(3)\simeq1.202056903$, the model gives $T_c\simeq209.5\,\mathrm{nK}$. At $T=0.8T_c\simeq167.6\,\mathrm{nK}$, $N_0/N=0.488$, or approximately $48\,800$ condensed [bosons](boson.md). These are chosen parameters and calculated values.

Finite $N$ gives a smooth crossover rather than a sharp [phase transition](phase-transition.md). The exact [ideal gas](ideal-gas-split.md) sum over excited [quantum harmonic oscillator](quantum-harmonic-oscillator-split.md) levels differs from the continuum integral, especially when $k_BT$ is not large relative to every $\hbar\omega_i$. A sharp trapped-gas limit takes $N\to\infty$, $\bar\omega\to0$ with $N\bar\omega^3$ fixed and fixed frequency ratios. Interactions also alter the [critical temperature](critical-temperature.md), [condensate fraction](condensate-fraction.md) and release profile; a dilute gas can have appreciable interaction [energy](energy-split.md) compared with the trap level spacing. The cubic law is a useful baseline, not a fit guaranteed for either 1995 experiment.

**Table of contents**

- [Harmonic-trap critical-temperature prefactor](harmonic-trap-critical-temperature-prefactor.md)
- [Saturation of harmonic-trap excited states](saturation-of-harmonic-trap-excited-states.md)
- [Harmonic-trap chemical-potential pinning](harmonic-trap-chemical-potential-pinning.md)
- [Harmonic-trap energy-zero convention](harmonic-trap-energy-zero-convention.md)
- [Condensate fraction](condensate-fraction.md)

## ↑ Ancestors (9)

1. [Dilute-gas Bose-Einstein condensation](dilute-gas-bose-einstein-condensation.md)
2. [Bose-Einstein condensation](bose-einstein-condensation.md)
3. [Bose-Einstein distribution](bose-einstein-distribution.md)
4. [Bose-Einstein statistics](bose-einstein-statistics.md)
5. [Quantum ideal-gas statistics](quantum-ideal-gas-statistics-split.md)
6. [Statistical physics](statistical-physics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Classical grand potential in a harmonic trap](classical-grand-potential-in-a-harmonic-trap.md)
- [Dilute-gas Bose-Einstein condensation](dilute-gas-bose-einstein-condensation.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2004/section-c/c12/solution.md)

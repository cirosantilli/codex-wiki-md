# Velocity relaxation time

↑ **Parent:** [Langevin dynamics](langevin-dynamics.md)

For a particle of [mass](mass.md) $m$ with [linear drag](linear-drag.md) $-\zeta v$, the velocity relaxation time is the [exponential relaxation time](exponential-relaxation-time.md) $\tau_v=m/\zeta$. Under a constant applied [force](force-split.md) $F$ and zero-mean random forcing, the averaged [Langevin equation](langevin-dynamics.md) is $m\,d\langle v\rangle/dt=-\zeta\langle v\rangle+F$. Solving gives

$$
\langle v(t)\rangle-\frac{F}{\zeta}=\left(\langle v(0)\rangle-\frac{F}{\zeta}\right)e^{-t/\tau_v}.
$$

Thus the initial mean-velocity deviation decays by a factor $e^{-1}$ after time $\tau_v$. Since the force-per-velocity coefficient $\zeta$ has units $\mathrm{kg\,s^{-1}}$, $m/\zeta$ has units of time. If the damping parameter is instead defined as a rate $\gamma=\zeta/m$, the same time is $1/\gamma$. For a sphere obeying [Stokes's law](stokes-s-law.md), $\tau_v=m/(6\pi\eta R)$. The [fluctuation-dissipation relation for a Langevin particle](fluctuation-dissipation-relation-for-a-langevin-particle.md) gives the same decay time for its equilibrium velocity [covariance](covariance.md).

## ↑ Ancestors (7)

1. [Langevin dynamics](langevin-dynamics.md)
2. [Stochastic process](stochastic-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Mean displacement](mean-displacement.md)
- [Mechanical mobility](mechanical-mobility.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2019/section-a/2/solution.md)

<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In [SI](../../../../international-system-of-units.md) units, the [Maxwell equations](../../../../maxwell-equations-split.md) in [vacuum](../../../../vacuum.md) with prescribed [charge density](../../../../charge-density.md) $\rho$ and [current density](../../../../current-density.md) $\mathbf J$ are

$$
\nabla\cdot\mathbf E=\frac\rho{\epsilon_0},\qquad
\nabla\cdot\mathbf B=0,\qquad
\nabla\times\mathbf E=-\partial_t\mathbf B,\qquad
\nabla\times\mathbf B=\mu_0\mathbf J+\mu_0\epsilon_0\partial_t\mathbf E.
$$

When $\rho=0$ and $\mathbf J=\mathbf0$, take the [curl](../../../../curl.md) of the third equation and substitute the fourth. Using the [curl of the curl identity](../../../../curl-of-the-curl-identity.md) and $\nabla\cdot\mathbf E=0$ gives the [electromagnetic wave equation](../../../../electromagnetic-wave-equation.md):

$$
\nabla\times(\nabla\times\mathbf E)=-\nabla^2\mathbf E
=-\mu_0\epsilon_0\partial_t^2\mathbf E,\qquad
\boxed{\nabla^2\mathbf E-\frac1{c^2}\partial_t^2\mathbf E=0,
\quad c=(\mu_0\epsilon_0)^{-1/2}.}
$$

For example, $\mathbf E=E_0\widehat{\mathbf x}\cos(kz-\omega t)$, $\mathbf B=(E_0/c)\widehat{\mathbf y}\cos(kz-\omega t)$ is a [plane electromagnetic wave](../../../../plane-electromagnetic-wave.md) provided $\omega=ck$. The [electric field](../../../../electric-field-split.md), [magnetic field](../../../../magnetic-field-split.md) and propagation direction are mutually perpendicular.

The [Maxwell equations](../../../../maxwell-equations-split.md) are linear, so the [superposition principle](../../../../superposition-principle.md) applies to fields. However, the [Poynting vector](../../../../poynting-vector.md) is quadratic:

$$
\langle\mathbf S\rangle=\frac1{\mu_0}\langle
\mathbf E_1\times\mathbf B_1+\mathbf E_2\times\mathbf B_2
+\mathbf E_1\times\mathbf B_2+\mathbf E_2\times\mathbf B_1\rangle.
$$

One may add the average [wave intensities](../../../../intensity-physics.md) only when the cross terms vanish under the actual detector average. For co-propagating [plane electromagnetic waves](../../../../plane-electromagnetic-wave.md) of parallel [linear polarization](../../../../linear-polarization.md), averaging over optical cycles but potentially resolving the difference [frequency](../../../../frequency.md) gives

$$
I(t)=I_1+I_2+2\sqrt{I_1I_2}\cos[(\omega_1-\omega_2)t+\phi].
$$

If the detector integrates for $T$, the last term acquires $\operatorname{sinc}[(\omega_1-\omega_2)T/2]$, with [sinc function](../../../../sinc-function.md) convention $\operatorname{sinc}x=\sin x/x$, evaluated at the midpoint phase. Thus $T\gg1/|f_1-f_2|$ suppresses [beats](../../../../beat.md), and the infinite-time average adds the [wave intensities](../../../../intensity-physics.md) exactly for distinct fixed [frequencies](../../../../frequency.md). Random mutually uncorrelated [wave phases](../../../../phase-waves.md) also remove the cross terms in an ensemble average; orthogonal [linear polarizations](../../../../linear-polarization.md) remove them for co-propagating waves in polarization-insensitive detection. Merely having different [frequencies](../../../../frequency.md) does not remove a resolved [beat](../../../../beat.md) signal: two nearly equal [frequencies](../../../../frequency.md) with fixed relative [wave phase](../../../../phase-waves.md) are a concrete counterexample. For different propagation directions, the relevant addition is of average [Poynting vectors](../../../../poynting-vector.md), or their components through the chosen detector [surface](../../../../topological-surface-split.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [2021 resit](../../../2021-resit-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

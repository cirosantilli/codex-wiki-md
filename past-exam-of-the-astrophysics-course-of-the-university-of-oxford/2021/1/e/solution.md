<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Retain the consistent $\Theta_{\rm phys}$ of [d](../d.md). Across a sufficiently thin layer, the neutral hydrogen [column density](../../../../column-density.md) is $N_{\rm HI}=n_H(1-\zeta_{\rm in})\Delta r+O(\Delta r^2)$. The direct stellar continuum acquires [optical depth](../../../../optical-depth.md) $\tau_\nu=N_{\rm HI}\sigma_\nu$. Define the photon-weighted second moment

$$
\langle\sigma^2\rangle=\frac1Q\int_0^\infty\sigma_\nu^2\frac{L_\nu^*}{h\nu}\,d\nu.
$$

Expanding the attenuating exponential in the [photoionization rate](../../../../photoionization-rate.md) gives

$$
\begin{aligned}
\frac{q(r_{\rm in}+\Delta r)}{q_{\rm in}}
&=\left(\frac{r_{\rm in}}{r_{\rm in}+\Delta r}\right)^2
\frac{\int\sigma_\nu L_\nu^*e^{-N_{\rm HI}\sigma_\nu}/(h\nu)\,d\nu}{Q\langle\sigma\rangle}\\
&=1-\frac{2\Delta r}{r_{\rm in}}-n_H(1-\zeta_{\rm in})\Delta r
\frac{\langle\sigma^2\rangle}{\langle\sigma\rangle}+O(\Delta r^2).
\end{aligned}
$$

The second [cross section](../../../../cross-section-physics.md) moment appears because the radiation both undergoes absorption and is weighted by the [photoionization](../../../../photoionization.md) [cross section](../../../../cross-section-physics.md) in computing the rate.

In a local plane-parallel approximation that suppresses geometrical dilution, set

$$
\Gamma=1-n_H(1-\zeta_{\rm in})\Delta r\frac{\langle\sigma^2\rangle}{\langle\sigma\rangle}.
$$

Then local [photoionization equilibrium](../../../../photoionization-equilibrium.md) becomes $\Theta_{\rm phys}\zeta^2=\Gamma(1-\zeta)$, so

$$
\boxed{\zeta=\frac{-\Gamma+\sqrt{\Gamma^2+4\Theta_{\rm phys}\Gamma}}{2\Theta_{\rm phys}}.}
$$

This gives the requested algebraic dependence, with the corrected definition of $\Theta$. Besides $\Delta r\ll r_{\rm in}$, linear attenuation requires $N_{\rm HI}\sigma_\nu\ll1$ over the [frequencies](../../../../frequency.md) contributing appreciably to the rate. In particular $\Gamma$ must remain positive.

The source's $\Gamma$ neglects $-2\Delta r/r_{\rm in}$, which is also first order in layer thickness. A consistent spherical first-order answer uses $\Gamma_{\rm sph}=\Gamma-2\Delta r/r_{\rm in}$ in the same root. Neglecting dilution relative to absorption additionally requires $n_H(1-\zeta_{\rm in})\langle\sigma^2\rangle/\langle\sigma\rangle\gg2/r_{\rm in}$. As a concrete limiting test, with negligible absorption the source's $\Gamma=1$ predicts no change, while inverse-square dilution still decreases $q$ and thus $\zeta$.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the astrophysics course of the University of Oxford](../../../split.md)
5. [Astrophysics course of the University of Oxford](../../../../astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

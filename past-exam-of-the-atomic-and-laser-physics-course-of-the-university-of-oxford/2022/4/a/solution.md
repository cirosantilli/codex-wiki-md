<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Define $r=g_2/g_1$ and let $\sigma=\sigma_{21}(\omega)$ be the stimulated-[emission cross section](../../../../emission-cross-section.md), averaged over upper [magnetic sublevels](../../../../magnetic-sublevel.md). The [Einstein coefficients](../../../../einstein-coefficients.md) relation $g_1B_{12}=g_2B_{21}$ gives the [absorption cross section](../../../../absorption-cross-section.md) $\sigma_{12}=r\sigma$. Assume equally populated [magnetic sublevels](../../../../magnetic-sublevel.md) within each [energy level](../../../../energy-level.md), a steady pump, and a monochromatic beam. The photon flux is $I/(\hbar\omega)$; define $W=\sigma I/(\hbar\omega)$ and the effective [population inversion](../../../../population-inversion.md) $D=N_2-rN_1$. Then the [rate equations](../../../../rate-equation.md) are

$$
\boxed{\dot N_2=R_2-A_{21}N_2-WD,\qquad
\dot N_1=A_{21}N_2+WD-\frac{N_1}{\tau_1}.}
$$

The $WD$ term includes both [stimulated emission](../../../../stimulated-emission.md) and [absorption](../../../../absorption-electromagnetic-radiation.md). In steady state, adding the two [rate equations](../../../../rate-equation.md) gives $N_1=R_2\tau_1$. The first equation then yields

$$
N_2=\frac{R_2+WrR_2\tau_1}{A_{21}+W},\qquad
D=\frac{R_2(1-rA_{21}\tau_1)}{A_{21}+W}.
$$

The directed beam gains [energy](../../../../energy-split.md) at rate $\hbar\omega WD$ per volume, giving $dI/dz=\sigma DI$ and the [optical gain](../../../../optical-gain.md) coefficient $\alpha=\sigma D$. At line centre, write $\sigma_0=\sigma_{21}(\omega_{21})$. Therefore

$$
\boxed{\alpha=\frac{\alpha_0}{1+I/I_s},\qquad
\alpha_0=\sigma_0R_2\left(\frac1{A_{21}}-r\tau_1\right),\qquad
I_s=\frac{\hbar\omega_{21}A_{21}}{\sigma_0}.}
$$

Here $\alpha_0$ is the small-signal [optical gain](../../../../optical-gain.md) coefficient and $I_s$ is the [saturation intensity](../../../../saturation-intensity.md), at which the local [optical gain](../../../../optical-gain.md) is half its small-signal value. Positive [optical gain](../../../../optical-gain.md) requires $rA_{21}\tau_1<1$: the lower [energy level](../../../../energy-level.md) must empty sufficiently quickly.

The cancellation of $\tau_1$ from $I_s$ is specific to this model's steady fixed pump and the fact that **every upper [spontaneous emission](../../../../spontaneous-emission.md) feeds the lower [energy level](../../../../energy-level.md)**. Adding an extra lower-state accumulation factor to $I_s$ would contradict these [rate equations](../../../../rate-equation.md). Alternative conventions using the [absorption cross section](../../../../absorption-cross-section.md) must replace $\sigma_0$ by $\sigma_{12}/r$ throughout. [Homogeneous spectral broadening](../../../../homogeneous-spectral-broadening.md) permits the whole selected ensemble to share this local [saturation](../../../../homogeneity-plus-realization-of-empty-set-types-implies-saturation.md) response.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the atomic and laser physics course of the University of Oxford](../../../split.md)
5. [Atomic and laser physics course of the University of Oxford](../../../../atomic-and-laser-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

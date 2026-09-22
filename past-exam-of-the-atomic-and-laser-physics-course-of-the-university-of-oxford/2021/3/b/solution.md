<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the energy-density convention of part (a), a normalized common [spectral line profile](../../../../spectral-line-profile.md) $\int\phi(\nu)\,d\nu=1$, and isotropic [spontaneous emission](../../../../spontaneous-emission.md). For a narrow [spectral line](../../../../spectral-line.md) centered at $\nu_0$,

$$
j_\nu=\frac{h\nu_0}{4\pi}n_2A_{21}\phi(\nu),\qquad
\kappa_\nu=\frac{h\nu_0}{c}(n_1B_{12}-n_2B_{21})\phi(\nu).
$$

The factor $1/c$ follows from $u_\nu=4\pi J_\nu/c$: angle-integrated absorption removes $c\kappa_\nu u_\nu$ of [energy](../../../../energy-split.md) per volume and time. The [emission coefficient](../../../../emission-coefficient.md) is per [solid angle](../../../../solid-angle.md), whereas the [absorption coefficient](../../../../absorption-coefficient.md) has units of inverse length.

The [Boltzmann distribution](../../../../boltzmann-distribution.md) in [thermal equilibrium](../../../../thermal-equilibrium-split.md) gives $n_2/n_1=(g_2/g_1)e^{-h\nu_0/(k_BT)}$. Dividing the two expressions and using the relations between [Einstein coefficients](../../../../einstein-coefficients.md),

$$
\begin{aligned}
S_\nu&=\frac{c}{4\pi}\frac{n_2A_{21}}{n_1B_{12}-n_2B_{21}}\\
&=\frac{2h\nu_0^3/c^2}{e^{h\nu_0/(k_BT)}-1}
=B_{\nu_0}(T).
\end{aligned}
$$

Thus the [source function](../../../../radiative-transfer-source-function.md) equals the [Planck function](../../../../planck-function.md) at the transition [frequency](../../../../frequency.md), and in the usual narrow-line approximation

$$
\boxed{S_\nu=B_\nu(T).}
$$

With an exactly common finite-width $\phi$ and constant line-center [Einstein coefficients](../../../../einstein-coefficients.md), their ratio is constant across the profile; exact equality to a varying $B_\nu$ at every frequency is only a narrow-line approximation. Exact thermal [radiative transfer](../../../../radiative-transfer.md) requires frequency-resolved [detailed balance](../../../../detailed-balance.md), which supplies the corresponding small profile corrections. This distinction does not alter the intended equilibrium result.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the atomic and laser physics course of the University of Oxford](../../../split.md)
5. [Atomic and laser physics course of the University of Oxford](../../../../atomic-and-laser-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

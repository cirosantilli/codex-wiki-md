<h1 id="section-d/d9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Debye model](../../../../../../debye-model.md) approximates a three-dimensional crystal as an elastic continuum supporting quantized [normal modes](../../../../../../normal-mode.md), or [phonons](../../../../../../phonon.md). At long [wavelengths](../../../../../../wavelength.md), the [acoustic phonon branches](../../../../../../acoustic-phonon-branch.md) have approximately linear [dispersion relations](../../../../../../dispersion-relation-split.md) $\omega_s(k)=v_s k$: one longitudinal branch and two transverse branches. Replace their complicated actual spectra by these linear forms, then introduce a cutoff chosen to preserve the total $3N$ vibrational degrees of freedom for $N$ atoms. This is an approximation to the spectrum, not a claim that a real crystal has no non-acoustic branches.

For [periodic boundary conditions](../../../../../../periodic-boundary-conditions.md) in [volume](../../../../../../volume.md) $V$, each allowed [wavevector](../../../../../../wavevector.md) occupies $(2\pi)^3/V$ in the space of [wavevectors](../../../../../../wavevector.md). Counting a spherical shell for each branch gives the [density of states](../../../../../../density-of-states.md) per unit [angular frequency](../../../../../../angular-frequency.md)

$$
g(\omega)=\frac{V\omega^2}{2\pi^2}\left(\frac1{v_l^3}+\frac2{v_t^3}\right).
$$

An effective [speed of sound](../../../../../../speed-of-sound.md) $v_D$ can be defined by $3/v_D^3=1/v_l^3+2/v_t^3$. In the single-speed [Debye model](../../../../../../debye-model.md), choose $\omega_D=v_Dk_D$ so that

$$
\int_0^{\omega_D}g(\omega)\,d\omega=3N.
$$

Thus the [Debye wavevector](../../../../../../debye-wavevector.md), [Debye frequency](../../../../../../debye-frequency.md) and [Debye temperature](../../../../../../debye-temperature.md) satisfy

$$
\boxed{k_D=\left(\frac{6\pi^2N}{V}\right)^{1/3},\qquad
\omega_D=v_Dk_D,\qquad \Theta_D=\frac{\hbar\omega_D}{k_B},\qquad
g(\omega)=\frac{9N\omega^2}{\omega_D^3}\quad(0<\omega<\omega_D).}
$$

Here $g$ has units of seconds when [angular frequency](../../../../../../angular-frequency.md) is measured in $\mathrm{s^{-1}}$; its integral is the dimensionless number of [normal modes](../../../../../../normal-mode.md). The spherical cutoff replaces the real [Brillouin zone](../../../../../../brillouin-zone.md) by an equal-count continuum construction.

Each [phonon](../../../../../../phonon.md) mode is a [quantum harmonic oscillator](../../../../../../quantum-harmonic-oscillator-split.md). Since [phonon](../../../../../../phonon.md) number is not conserved at [thermal equilibrium](../../../../../../thermal-equilibrium-split.md), the [chemical potential](../../../../../../chemical-potential-split.md) is zero and its [Bose-Einstein distribution](../../../../../../bose-einstein-distribution.md) gives mean thermal [energy](../../../../../../energy-split.md) $\hbar\omega/[e^{\hbar\omega/(k_BT)}-1]$. The [zero-point energy](../../../../../../zero-point-energy.md) is independent of [temperature](../../../../../../temperature-split.md) in the harmonic, fixed-volume approximation and does not contribute to the [heat capacity at constant volume](../../../../../../heat-capacity-at-constant-volume.md). Excluding that constant term,

$$
U(T)=\int_0^{\omega_D}\frac{g(\omega)\hbar\omega}{e^{\hbar\omega/(k_BT)}-1}\,d\omega
=9Nk_BT\left(\frac{T}{\Theta_D}\right)^3
\int_0^{\Theta_D/T}\frac{x^3}{e^x-1}\,dx.
$$

Differentiating the first [integral](../../../../../../integral-split.md) at fixed [volume](../../../../../../volume.md) avoids losing the temperature-dependent upper limit in the second one. The resulting [Debye heat capacity](../../../../../../debye-heat-capacity.md) is

$$
\boxed{C_V=9Nk_B\left(\frac{T}{\Theta_D}\right)^3
\int_0^{\Theta_D/T}\frac{x^4e^x}{(e^x-1)^2}\,dx.}
$$

For $T\ll\Theta_D$, extend the upper limit to infinity. Expanding $1/(e^x-1)=\sum_{r\ge1}e^{-rx}$ and integrating term by term gives $\int_0^\infty x^3/(e^x-1)\,dx=6\zeta(4)=\pi^4/15$. Therefore

$$
U\simeq\frac{3\pi^4}{5}Nk_B\frac{T^4}{\Theta_D^3},\qquad
\boxed{C_V\simeq\frac{12\pi^4}{5}Nk_B\left(\frac{T}{\Theta_D}\right)^3.}
$$

This $T^3$ law follows from the three-dimensional $\omega^2$ [density of states](../../../../../../density-of-states.md) and the availability only of low-[frequency](../../../../../../frequency.md) modes at low [temperature](../../../../../../temperature-split.md). It is a central success of the [Debye model](../../../../../../debye-model.md).

For $T\gg\Theta_D$, the [Bose-Einstein distribution](../../../../../../bose-einstein-distribution.md) reduces to the classical [equipartition theorem](../../../../../../equipartition-theorem.md): every mode contributes thermal [energy](../../../../../../energy-split.md) $k_BT$. Consequently

$$
\boxed{U\simeq3Nk_BT,\qquad C_V\longrightarrow3Nk_B,}
$$

the [Dulong-Petit law](../../../../../../dulong-petit-law.md), or $3R$ per mole of atoms. The simple model omits detailed [phonon dispersion relation](../../../../../../phonon-dispersion-relation.md), distinct [optical phonon branches](../../../../../../optical-phonon-branch.md), and anharmonic effects such as [thermal expansion](../../../../../../thermal-expansion.md). In a [metal](../../../../../../metal.md), the low-[temperature](../../../../../../temperature-split.md) total [heat capacity](../../../../../../heat-capacity.md) additionally contains a term approximately proportional to $T$ from [electrons](../../../../../../electron.md), so the lattice $T^3$ term should not be mistaken for the whole measurement.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [D9](../../d9.md)
3. [Section D](../../../section-d.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)

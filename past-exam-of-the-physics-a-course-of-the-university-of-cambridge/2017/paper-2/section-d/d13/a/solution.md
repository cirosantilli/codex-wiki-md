<h1 id="section-d/d13/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Debye model](../../../../../../debye-model.md) treats a solid's low-frequency lattice vibrations as acoustic [phonons](../../../../../../phonon.md) in an elastic continuum. There are three polarizations per [wavevector](../../../../../../wavevector.md), one longitudinal and two transverse, with approximately linear [dispersion relations](../../../../../../dispersion-relation-split.md). A cutoff is chosen to preserve the total $3N$ vibrational modes of $N$ atoms. The [phonon](../../../../../../phonon.md) number itself is not fixed; mode occupations follow the [Bose-Einstein distribution](../../../../../../bose-einstein-distribution.md) with zero [chemical potential](../../../../../../chemical-potential-split.md).

For one polarization of speed $v_s$, counting [wavevector](../../../../../../wavevector.md) states in a spherical shell gives $g_s(\omega)=V\omega^2/(2\pi^2v_s^3)$. Define an average Debye speed by $3/v_D^3=1/v_L^3+2/v_T^3$. The total [density of states](../../../../../../density-of-states.md) can then be written

$$
g(\omega)=\frac{9N\omega^2}{\omega_D^3},\quad0\leq\omega\leq\omega_D,\qquad
\int_0^{\omega_D}g(\omega)d\omega=3N.
$$

The [Debye wavevector](../../../../../../debye-wavevector.md) is $k_D=(6\pi^2N/V)^{1/3}$, the [Debye frequency](../../../../../../debye-frequency.md) is $\omega_D=v_Dk_D$, and the [Debye temperature](../../../../../../debye-temperature.md) is $\Theta_D=\hbar\omega_D/k_B$.

Omitting the temperature-independent [zero-point energy](../../../../../../zero-point-energy.md), the vibrational [energy](../../../../../../energy-split.md) and resulting [Debye heat capacity](../../../../../../debye-heat-capacity.md) are

$$
U=\int_0^{\omega_D}\frac{g(\omega)\hbar\omega}{e^{\hbar\omega/(k_BT)}-1}\,d\omega,\qquad
\boxed{C_V=9Nk_B\left(\frac T{\Theta_D}\right)^3\int_0^{\Theta_D/T}\frac{x^4e^x}{(e^x-1)^2}\,dx}.
$$

At low [temperature](../../../../../../temperature-split.md) the upper limit can be extended to infinity. The integral is $4\pi^4/15$, giving

$$
\boxed{C_V\simeq\frac{12\pi^4}{5}Nk_B\left(\frac T{\Theta_D}\right)^3},\qquad T\ll\Theta_D.
$$

Only the long-wavelength acoustic modes are appreciably populated, explaining the [Debye T-cubed test](../../../../../../debye-t-cubed-test.md). At high [temperature](../../../../../../temperature-split.md) every mode contributes $k_B$ by [equipartition theorem](../../../../../../equipartition-theorem.md), so $\boxed{C_V\to3Nk_B}$, the [Dulong-Petit law](../../../../../../dulong-petit-law.md).

<a id="section-d/d13/a/image-debye-heat-capacity-approaching-its-classical-limit-and-its-low-temperature-cubic-law"></a>
![](../../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-2-d13-debye-heat-capacity.png)

**[Figure 7](#section-d/d13/a/image-debye-heat-capacity-approaching-its-classical-limit-and-its-low-temperature-cubic-law). Debye heat capacity approaching its classical limit and its low-temperature cubic law**.

The model succeeds especially at low [temperature](../../../../../../temperature-split.md), where long-wavelength elasticity is reliable. It replaces real anisotropic branches by a simple continuum and cannot reproduce detailed [optical phonon branches](../../../../../../optical-phonon-branch.md) or every intermediate-temperature feature. Metals also have an [electronic heat capacity](../../../../../../electronic-heat-capacity.md) approximately proportional to $T$; defects, magnetic excitations or a [phase](../../../../../../phase-waves.md) transition can add other terms. Experiments often measure [heat capacity at constant pressure](../../../../../../heat-capacity-at-constant-pressure.md), which need not equal the harmonic model's $C_V$ exactly.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2017](../../../../split.md)
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

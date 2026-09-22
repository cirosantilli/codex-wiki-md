<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Measure energies from the single-particle [ground state](../../../../ground-state.md), and assume the **three-dimensional ideal Bose gas in the large-particle-number limit**. The [harmonic-trap chemical-potential pinning](../../../../harmonic-trap-chemical-potential-pinning.md) discussed here uses a [chemical potential](../../../../chemical-potential-split.md) satisfying $\mu_{\rm ch}\leq0$. On cooling, it approaches zero; below the condensation [temperature](../../../../temperature-split.md) it remains at zero to leading thermodynamic order. Above that [temperature](../../../../temperature-split.md) it is negative. The detailed negative-chemical-potential branch shape is determined by the [density of states](../../../../density-of-states.md); the figure uses the harmonic trap analysed below. The [finite-size condensate chemical potential](../../../../finite-size-condensate-chemical-potential.md) stays slightly below zero rather than being exactly pinned there.

A **[Bose-Einstein condensate](../../../../bose-einstein-condensate.md) has macroscopic occupation of a single quantum state**. A dilute atomic gas needs low [temperature](../../../../temperature-split.md) and high phase-space [density](../../../../density.md) while remaining metastable against ordinary liquid or solid formation. [Laser cooling](../../../../laser-cooling.md) followed by [evaporative cooling of atoms](../../../../evaporative-cooling-atomic-physics.md) in a weak trap can achieve the required regime. For the trapped ideal gas the quantitative threshold is derived below; a uniform ideal gas has $n\lambda_T^3=\zeta(3/2)$ at onset. An experimental signature is a narrow low-momentum component appearing within the broader thermal distribution after time-of-flight expansion, as observed in magnetically trapped rubidium-87.[1995 rubidium experiment: low-velocity condensate component and nonthermal anisotropic expansion](../../../../observation-of-bose-einstein-condensation-in-a-dilute-atomic-vapor-by-m-h-anderson-and-others.md)

**[Spinless cubic-box wave-vector counting](../../../../spinless-cubic-box-wave-vector-counting.md).** Impose [periodic boundary conditions](../../../../periodic-boundary-conditions.md) on a cube of side $L$. The allowed vectors are $\mathbf k=(2\pi/L)(n_x,n_y,n_z)$ with integer components. Each state occupies $ (2\pi/L)^3$ in wave-vector space. For a spinless particle, counting the spherical shell gives

$$
d\mathcal N=\frac{V}{(2\pi)^3}4\pi k^2dk,\qquad\boxed{g_V(k)=\frac1V\frac{d\mathcal N}{dk}=\frac{k^2}{2\pi^2}.}
$$

There is no [spin](../../../../spin.md) multiplicity. This is continuum shell counting; a finite box has discrete levels. Using $\epsilon=\hbar^2k^2/(2m)$ gives the free-particle [density of states](../../../../density-of-states.md) per unit [energy](../../../../energy-split.md) and [volume](../../../../volume.md)

$$
g_V(\epsilon)=\frac{(2m)^{3/2}}{4\pi^2\hbar^3}\sqrt\epsilon.
$$

**[Semiclassical density of states in a central potential](../../../../semiclassical-density-of-states-in-a-central-potential.md).** At position $\mathbf r$, the available [kinetic energy](../../../../kinetic-energy.md) is $\epsilon-U(r)$. The local-density approximation integrates the preceding free-particle result over the classically allowed region:

$$
g(\epsilon)=\int_{U<\epsilon}\frac{(2m)^{3/2}}{4\pi^2\hbar^3}\sqrt{\epsilon-U(r)}\,d^3r=\boxed{\frac{(2m)^{3/2}}{\pi\hbar^3}\int_0^{r_\epsilon}r^2\sqrt{\epsilon-U(r)}\,dr.}
$$

This form assumes the allowed radial region is the connected interval $0\leq r\leq r_\epsilon$. A nonmonotonic potential would require integrating all allowed shells.

For the isotropic harmonic trap, $r_\epsilon=\sqrt{2\epsilon/(m\omega^2)}$. Substituting $r=r_\epsilon\sin\vartheta$ gives

$$
\int_0^{r_\epsilon}r^2\sqrt{\epsilon-\tfrac12m\omega^2r^2}\,dr=r_\epsilon^3\sqrt\epsilon\int_0^{\pi/2}\sin^2\vartheta\cos^2\vartheta\,d\vartheta=\frac\pi{16}r_\epsilon^3\sqrt\epsilon.
$$

Consequently

$$
\boxed{g(\epsilon)=\frac{\epsilon^2}{2(\hbar\omega)^3}.}
$$

The exact oscillator ground [energy](../../../../energy-split.md) is $3\hbar\omega/2$ above the potential minimum. The [harmonic-trap energy-zero convention](../../../../harmonic-trap-energy-zero-convention.md) subtracts that constant, while the displayed [density of states](../../../../density-of-states.md) is the leading semiclassical continuum expression, neglecting the finite-level corrections produced by that shift. The discrete [ground state](../../../../ground-state.md) must be counted separately.

**Condensate population.** Below the transition, use $\mu_{\rm ch}\simeq0$ for the excited states. The [saturation of harmonic-trap excited states](../../../../saturation-of-harmonic-trap-excited-states.md) follows from the supplied integral:

$$
N_{\rm ex}=\int_0^\infty\frac{g(\epsilon)\,d\epsilon}{e^{\epsilon/(k_BT)}-1}=\frac12\left(\frac{k_BT}{\hbar\omega}\right)^3\int_0^\infty\frac{x^2dx}{e^x-1}=\zeta(3)\left(\frac{k_BT}{\hbar\omega}\right)^3,
$$

where $\zeta$ is the [Riemann zeta function](../../../../riemann-zeta-function.md) and $\zeta(3)\simeq1.202$. Setting $N_{\rm ex}(T_0)=N$ gives the [harmonic-trap critical-temperature prefactor](../../../../harmonic-trap-critical-temperature-prefactor.md):

$$
\boxed{T_0=\frac{\hbar\omega}{k_B}\left(\frac N{\zeta(3)}\right)^{1/3}\simeq0.9405\frac{\hbar\omega}{k_B}N^{1/3},\qquad \frac{N_0(T)}N=1-\left(\frac T{T_0}\right)^3\quad(T<T_0).}
$$

Above $T_0$ there is no macroscopic ground-state fraction in this approximation. For completeness, above the transition the [quantum gas fugacity](../../../../fugacity-statistical-mechanics.md) $z=e^{\mu_{\rm ch}/(k_BT)}<1$ satisfies $N=(k_BT/\hbar\omega)^3\operatorname{Li}_3(z)$; the [polylogarithm](../../../../polylogarithm.md) $\operatorname{Li}_3$ therefore defines the plotted negative branch. A finite trapped gas has rounded behaviour, weak interactions shift the threshold, and the continuum thermal population is inaccurate when $k_BT$ is comparable to or below $\hbar\omega$. The power law is intended for the large-$N$ condensed regime, not an exact discrete-spectrum formula at arbitrarily small [temperature](../../../../temperature-split.md).[Section 3.5: Bose distribution, excited-state saturation and separate condensate population; trap density-of-states calculation derived here](../../../../quantum-gases-by-david-tong.md)

<a id="3/image-leading-ideal-harmonic-trap-chemical-potential-and-condensate-fraction-versus-temperature-with-energy-measured-from-the-ground-state"></a>
![](../../../../past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2016/paper-1-trapped-condensate.png)

**[Figure 6](#3/image-leading-ideal-harmonic-trap-chemical-potential-and-condensate-fraction-versus-temperature-with-energy-measured-from-the-ground-state). Leading ideal harmonic-trap chemical potential and condensate fraction versus temperature, with energy measured from the ground state**. [Source](paper-1-trapped-condensate.py).

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2016](../../split.md)
4. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../split.md)
5. [Thermal and Statistical Physics course of the University of Cambridge](../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)

<h1 id="section-c/c10/solution">Solution</h1>

↑ **Parent:** [C10](../c10.md)

The [free electron model](../../../../../free-electron-model.md) replaces the microscopic ionic potential and interacting electronic motion by independent mobile [electrons](../../../../../electron.md) in a uniform neutralizing background, with approximately parabolic dispersion $\epsilon=\hbar^2k^2/(2m^*)$. Its quantum version fills states according to [Fermi-Dirac statistics](../../../../../fermi-dirac-statistics.md) and the [Pauli exclusion principle](../../../../../pauli-exclusion-principle.md). Scattering is represented by a [momentum relaxation time](../../../../../momentum-relaxation-time.md) $\tau$, rather than derived from the model's ideal free trajectories. This model explains a [Fermi energy](../../../../../fermi-energy.md) much larger than room-temperature thermal [energy](../../../../../energy-split.md), an [electronic heat capacity](../../../../../electronic-heat-capacity.md) proportional to [temperature](../../../../../temperature-split.md) at low [temperature](../../../../../temperature-split.md), and a Drude [electrical conductivity](../../../../../electrical-conductivity.md). With appropriate scattering assumptions it also yields the [Wiedemann-Franz law](../../../../../wiedemann-franz-law.md). It cannot by itself explain [band gaps](../../../../../band-gap.md), detailed band anisotropy, strong correlations, or the microscopic [temperature](../../../../../temperature-split.md) dependence of $\tau$.

The inertial term is [mass](../../../../../mass.md) times the rate of change of mean [drift velocity](../../../../../drift-velocity.md). The electric [force](../../../../../force-split.md) is $eE$, taking the printed $e$ as the signed [electron](../../../../../electron.md) charge, and $-\gamma\langle v\rangle=-m^*\langle v\rangle/\tau$ describes loss of directed momentum to scattering. [electrons](../../../../../electron.md) retain large microscopic [velocities](../../../../../velocity.md); this [damping](../../../../../damping.md) is of their mean directed motion. In a steady DC field,

$$
\langle v\rangle=\frac{e\tau}{m^*}E,\qquad
j=ne\langle v\rangle,\qquad
\boxed{\sigma_0=\frac{ne^2\tau}{m^*}.}
$$

Both charge factors are negative for [electrons](../../../../../electron.md), so the conductivity is positive. If $e$ instead denotes a positive charge magnitude, the [force](../../../../../force-split.md) and current equations each require a minus sign and give the same result.

For AC response choose physical fields as [real parts](../../../../../real-part.md) of [phasors](../../../../../phasor.md) proportional to $e^{-i\omega t}$. Substitution gives

$$
(-i\omega+1/\tau)\widehat v=\frac{e}{m^*}\widehat E,\qquad
\boxed{\sigma(\omega)=\frac{\sigma_0}{1-i\omega\tau}.}
$$

Thus

$$
\boxed{\operatorname{Re}\sigma=\frac{\sigma_0}{1+(\omega\tau)^2},\qquad
\operatorname{Im}\sigma=\frac{\sigma_0\omega\tau}{1+(\omega\tau)^2}.}
$$

The [real part](../../../../../real-part.md) decreases from $\sigma_0$ to zero. The [imaginary part](../../../../../imaginary-part.md) starts at zero, reaches $\sigma_0/2$ at $\omega\tau=1$, and falls as $1/\omega$. The [real part](../../../../../real-part.md) falls as $1/\omega^2$ at high [frequency](../../../../../frequency.md). With an $e^{+i\omega t}$ convention, only the sign of the [imaginary part](../../../../../imaginary-part.md) changes. Positive $\operatorname{Re}\sigma$ gives positive cycle-averaged dissipation $\langle jE\rangle=\operatorname{Re}\sigma\,|\widehat E|^2/2$.

<a id="section-c/c10/image-drude-conductivity-and-the-dispersion-and-density-of-states-of-a-monatomic-harmonic-chain"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-2-drude-chain.png)

**[Figure 4](#section-c/c10/image-drude-conductivity-and-the-dispersion-and-density-of-states-of-a-monatomic-harmonic-chain). Drude conductivity and the dispersion and density of states of a monatomic harmonic chain**.

The supplied DC conductivity determines the transport time:

$$
\tau=\frac{m_e\sigma_0}{ne^2}=2.49\times10^{-14}\,\mathrm s.
$$

Inertia matters when $\omega\tau\sim1$, giving **$\omega_c\simeq4.02\times10^{13}\,\mathrm{rad\,s^{-1}}$**, or **$\nu_c=\omega_c/(2\pi)\simeq6.40\times10^{12}\,\mathrm{Hz}$**. Quoting the former number as hertz would introduce an erroneous factor of $2\pi$.

## ↑ Ancestors (14)

1. [C10](../c10.md)
2. [Section C](../../section-c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)

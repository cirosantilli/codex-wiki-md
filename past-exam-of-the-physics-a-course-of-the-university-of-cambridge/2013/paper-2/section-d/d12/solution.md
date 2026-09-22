<h1 id="section-d/d12/solution">Solution</h1>

↑ **Parent:** [D12](../d12.md)

The [Debye model](../../../../../debye-model.md) replaces the crystal by a harmonic elastic continuum with acoustic dispersion $\omega=v_sk$. It counts three [polarizations](../../../../../polarization-waves.md) and introduces a cutoff so that the total number of vibrational modes is $3N$, where $N$ is the atom count. Periodic-box counting gives

$$
g(\omega)=\frac{V\omega^2}{2\pi^2}\left(\frac1{v_L^3}+\frac2{v_T^3}\right).
$$

For an isotropic average speed, $3/v_D^3=1/v_L^3+2/v_T^3$. With cutoff [frequency](../../../../../frequency.md) $\omega_D$ fixed by the mode count,

$$
\boxed{g(\omega)=\frac{9N\omega^2}{\omega_D^3}\quad(0<\omega<\omega_D),\qquad
\Theta_D=\frac{\hbar\omega_D}{k_B}}.
$$

This [density of states](../../../../../density-of-states.md) is quadratic because a three-dimensional shell has [volume](../../../../../volume.md) proportional to $k^2dk$ and the acoustic dispersion is linear. The cutoff is a mode-counting device; it is not a claim that every actual branch stays linear to the zone boundary.

Each [phonon](../../../../../phonon.md) mode has mean thermal [energy](../../../../../energy-split.md) $\hbar\omega/(e^{\beta\hbar\omega}-1)$, using [Bose-Einstein statistics](../../../../../bose-einstein-statistics.md) with zero [phonon](../../../../../phonon.md) [chemical potential](../../../../../chemical-potential-split.md). The fixed harmonic zero-point contribution has zero [temperature](../../../../../temperature-split.md) [derivative](../../../../../derivative.md). With $x=\hbar\omega/(k_BT)$,

$$
U_{\rm th}=9Nk_BT\left(\frac{T}{\Theta_D}\right)^3
\int_0^{\Theta_D/T}\frac{x^3}{e^x-1}dx,
$$

and differentiating at fixed [volume](../../../../../volume.md) gives

$$
\boxed{C_V=9Nk_B\left(\frac{T}{\Theta_D}\right)^3
\int_0^{\Theta_D/T}\frac{x^4e^x}{(e^x-1)^2}dx}.
$$

For $T\ll\Theta_D$, extend the upper limit to infinity. Expanding $1/(e^x-1)=\sum_{j\geq1}e^{-jx}$ gives $\int_0^\infty x^3/(e^x-1)dx=6\sum j^{-4}=\pi^4/15$. [integration](../../../../../integral-split.md) by parts makes the heat-capacity [integral](../../../../../integral-split.md) $4\pi^4/15$, so

$$
\boxed{C_V\simeq\frac{12\pi^4}{5}Nk_B\left(\frac T{\Theta_D}\right)^3}.
$$

Only modes with $\hbar\omega\lesssim k_BT$ are appreciably excited; their number scales as $T^3$, explaining the [power](../../../../../power.md) law physically. At high [temperature](../../../../../temperature-split.md) every mode contributes $k_B$, giving the Dulong-Petit limit $C_V\to3Nk_B$.

The model assumes the [harmonic approximation](../../../../../harmonic-approximation.md), a macroscopic three-dimensional solid and acoustic continuum behaviour for the thermally populated modes. Anisotropic [sound speeds](../../../../../speed-of-sound.md) change the low-temperature coefficient rather than its cubic [power](../../../../../power.md). Real optical branches and nonlinear acoustic dispersion limit the full-temperature approximation; electronic excitations can add a linear term in a metal, and [anharmonicity](../../../../../anharmonicity.md) produces [thermal expansion](../../../../../thermal-expansion.md) and distinctions between $C_P$ and $C_V$. At [temperatures](../../../../../temperature-split.md) below the lowest finite-sample mode, the bulk continuum law also fails. Thus **the $T^3$ result is the low-temperature lattice contribution**, not a universal total [heat capacity](../../../../../heat-capacity.md) for every solid.

## ↑ Ancestors (14)

1. [D12](../d12.md)
2. [Section D](../../section-d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2013](../../../split.md)
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

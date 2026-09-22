<h1 id="section-a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The exponential factor removes the first spatial derivative. Apply the [chain rule](../../../../chain-rule.md) explicitly:

$$
\partial_z\Delta\rho=e^{-z/(2H)}\left(\Psi_z-\frac{\Psi}{2H}\right),\qquad
\partial_z^2\Delta\rho=e^{-z/(2H)}\left(\Psi_{zz}-\frac{\Psi_z}{H}+\frac{\Psi}{4H^2}\right),
$$

while $\partial_t^2\Delta\rho=e^{-z/(2H)}\Psi_{tt}$. Substituting into the supplied density equation, the terms proportional to $\Psi_z$ cancel, leaving

$$
\boxed{\Psi_{tt}-c^2\Psi_{zz}+\frac{c^2}{4H^2}\Psi=0,
\qquad \omega_0=\frac{c}{2H}.}
$$

This is the [atmospheric acoustic cutoff transformation](../../../../atmospheric-acoustic-cutoff-transformation.md). There is a sign error in the target equation in the original PDF, as well as in the transcription: the last term must be $+\omega_0^2\Psi$ for real positive $\omega_0$. If the displayed minus sign is retained literally, coefficient matching would require $\omega_0^2=-c^2/(4H^2)$, so it would not define a real characteristic oscillation period.

For the corrected equation, a [plane wave](../../../../plane-wave.md) $\Psi\propto e^{i(kz-\omega t)}$ has [dispersion relation](../../../../dispersion-relation-split.md)

$$
\omega^2=c^2k^2+\omega_0^2.
$$

Thus $\omega_0$ is the [acoustic cutoff frequency](../../../../acoustic-cutoff-frequency.md): vertically propagating [acoustic waves](../../../../acoustic-wave.md) have $|\omega|\ge\omega_0$. The [scale height](../../../../scale-height.md) and [sound speed](../../../../speed-of-sound.md) have units metres and metres per second, respectively, so $\omega_0$ has units $\mathrm{s^{-1}}$.

For an order-of-magnitude estimate in the lower [terrestrial atmosphere](../../../../terrestrial-atmosphere.md), take $H\simeq8.0\ \mathrm{km}$ and $c\simeq340\ \mathrm{m\,s^{-1}}$. These are representative atmospheric values, not additional data specified by the paper. They give

$$
\omega_0\simeq2.1\times10^{-2}\ \mathrm{s^{-1}},\qquad
\boxed{\frac{2\pi}{\omega_0}=\frac{4\pi H}{c}\simeq3.0\times10^2\ \mathrm s\simeq5\ \mathrm{min}.}
$$

The [isothermal atmosphere](../../../../isothermal-atmosphere.md) approximation is local: a real atmospheric [temperature](../../../../temperature-split.md) profile and the thermodynamic response of the disturbance modify the precise cutoff and period.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Section A](../../section-a.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../split.md)
5. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)

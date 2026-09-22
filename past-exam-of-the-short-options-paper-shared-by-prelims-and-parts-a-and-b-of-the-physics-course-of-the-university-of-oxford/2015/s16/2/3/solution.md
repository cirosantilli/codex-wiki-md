<h1 id="s16/2/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use collisional [inverse bremsstrahlung](../../../../../inverse-bremsstrahlung.md) in a weakly coupled, unmagnetized plasma. The specified density is $n_e=10^{26}\,\mathrm{m^{-3}}$, and $k_BT=1000\,\mathrm{eV}$. The electron [Debye length](../../../../../debye-length.md) is $2.35\times10^{-8}\,\mathrm m$, the [plasma frequency](../../../../../plasma-frequency.md) is $5.64\times10^{14}\,\mathrm{s^{-1}}$, and the laser angular frequency is $\omega=2\pi c/\lambda=1.79\times10^{15}\,\mathrm{s^{-1}}$. Thus $X=\omega_p^2/\omega^2\simeq0.099<1$: the plasma is underdense and a propagating wave exists.

Estimate $b_{\min}$ as the larger of the classical Coulomb-deflection length $Ze^2/(4\pi\epsilon_0k_BT)$ and the electron quantum length $\hbar/\sqrt{m_ek_BT}$. Both are about $9\times10^{-12}\,\mathrm m$ here, giving $\ln\Lambda_C\simeq8$. With the usual thermal collision convention,

$$
\nu_{ei}\simeq2.91\times10^{-6}\frac{n_e[\mathrm{cm^{-3}}]Z\ln\Lambda_C}{T_e[\mathrm{eV}]^{3/2}}\,\mathrm{s^{-1}}\simeq4.4\times10^{11}\,\mathrm{s^{-1}}.
$$

The $Z$ factor follows from $n_iZ^2=n_eZ$.[Coulomb collision-rate normalization and thermal parameters; densities in cubic centimetres and temperatures in eV](../../../../../nrl-plasma-formulary-2019.md)

The weakly collisional [Drude model](../../../../../drude-model.md) gives $\epsilon_r=1-\omega_p^2/[\omega(\omega+i\nu_{ei})]$ for fields proportional to $e^{-i\omega t}$. Expanding at $\nu_{ei}\ll\omega$ yields a real refractive index $n_r=\sqrt{1-X}\simeq0.949$ and intensity attenuation coefficient

$$
\alpha_I=2\operatorname{Im}k\simeq\frac{\nu_{ei}}{c}\frac{X}{\sqrt{1-X}}.
$$

Consequently the intensity e-folding absorption length is

$$
\boxed{L_I=\frac{c\sqrt{1-X}}{\nu_{ei}X}\simeq6.6\times10^{-3}\,\mathrm m,}
$$

i.e. of order a centimetre. Taking a Coulomb logarithm between about 5 and 10 gives roughly $5$–$10\,\mathrm{mm}$. The electric-field amplitude decay length is twice this intensity length. This estimate assumes a uniform slab thick enough to define an absorption length and neglects gradients, nonlinear quiver heating and other absorption mechanisms.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [2](../../2.md)
3. [S16](../../../s16.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

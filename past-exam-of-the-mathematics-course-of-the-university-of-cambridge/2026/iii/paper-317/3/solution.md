<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

In [stellar homology](../../../../../stellar-homology.md), two stars have identical dimensionless density, pressure, temperature, and luminosity profiles. Mass conservation, [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md), and the perfect-gas equation of state then give

$$
\boxed{\rho_c\propto\frac M{R^3}},
\qquad
\boxed{P_c\propto\frac{GM^2}{R^4}},
\qquad
\boxed{T_c\propto\frac{\mu GM}{R}}.
$$

The chemical composition is initially fixed here, so $\mu$ is constant.

For opacity $\kappa=\kappa_0\rho^aT^b$, radiative diffusion gives the homology scaling

$$
L_{\rm rad}\propto
\kappa_0^{-1}R T_c^{4-b}\rho_c^{-(a+1)}
\propto\kappa_0^{-1}M^{3-a-b}R^{3a+b}.
$$

Nuclear burning with $\epsilon=\epsilon_0\rho T^n$ instead gives

$$
L_{\rm nuc}\propto\epsilon_0M\rho_cT_c^n
\propto\epsilon_0M^{n+2}R^{-(n+3)}.
$$

Equating the two luminosities yields

$$
R\propto M^{(n-1+a+b)/(n+3+3a+b)}
$$

and the [mass-luminosity relation](../../../../../mass-luminosity-relation.md)

$$
\boxed{L\propto M^\eta},
\qquad
\boxed{\eta=\frac{2an+3a-b+3n+9}{n+3+3a+b}}.
$$

For usual main-sequence opacity and burning laws, $\eta>1$, so massive stars are much more luminous and exhaust a fuel supply proportional to $M$ in a time $t_*\propto M/L\propto M^{1-\eta}$.

At sufficiently high mass, radiation pressure and radiative acceleration become important. Hydrostatic balance requires the luminosity to remain below the [Eddington luminosity](../../../../../eddington-luminosity.md)

$$
\boxed{L_{\rm Edd}=\frac{4\pi cGM}{\kappa}}.
$$

The upper envelope is linear in $M$, so the relation must flatten toward slope one; the corresponding nuclear lifetime approaches a weakly mass-dependent or roughly constant value rather than continuing the steep decline predicted by gas-pressure homology.

During core hydrogen burning, conversion of hydrogen into helium reduces the number of free particles per unit mass and raises the mean molecular weight. The core contracts and heats to retain pressure support, while the envelope expands and the luminosity generally rises. Homology ultimately fails because composition becomes strongly nonuniform, an inert helium core and hydrogen-burning shell appear, and the core and envelope acquire qualitatively different equations of state, transport regimes, and radial scales as the star leaves the [main sequence](../../../../../main-sequence.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 317](../../paper-317-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

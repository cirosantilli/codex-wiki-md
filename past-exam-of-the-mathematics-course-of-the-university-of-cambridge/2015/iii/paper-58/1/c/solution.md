<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Since $\epsilon$ is per unit mass, each shell contributes $dL=\epsilon\,dm=4\pi r^2\rho\epsilon\,dr$. Both factors of [mass density](../../../../../../density.md) must be retained. Substituting the [linear-density stellar model](../../../../../../linear-density-stellar-model.md) and its [temperature](../../../../../../temperature.md) profile gives

$$
L(r)=4\pi\epsilon_0\rho_c^2R^3\left(\frac{T_c}{T_0}\right)^\nu\int_0^{r/R}x^2(1-x)^{2+\nu}\left(1+2x-\frac95x^2\right)^\nu\,dx.
$$

Writing $I_\nu(z)$ for this incomplete integral, with $I_\nu=I_\nu(1)$, the [luminosity](../../../../../../luminosity.md) is

$$
\boxed{L(r)=\frac{36\epsilon_0M^2}{\pi R^3}\left(\frac{5GM}{12\mathcal R RT_0}\right)^\nu I_\nu(r/R),\qquad L(R)=\frac{36\epsilon_0M^2}{\pi R^3}\left(\frac{5GM}{12\mathcal R RT_0}\right)^\nu I_\nu.}
$$

This supplies both the local $L_r$ and the total [luminosity](../../../../../../luminosity.md) associated with the printed integral extending to one. For fixed composition and fixed $\nu$, the total scales as $M^{2+\nu}R^{-3-\nu}$. The physical nuclear-heating exponents are positive; mathematically the surface integral converges for $\nu>-3$. As a simple normalization check, $I_0=1/30$, hence $L(R)=6\epsilon_0M^2/(5\pi R^3)$ for temperature-independent heating. This is the generated [luminosity](../../../../../../luminosity.md); the radiative-transport incompatibility noted above is not removed by integrating the heating.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

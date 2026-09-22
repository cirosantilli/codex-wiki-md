<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take upward deflection as positive, use $k>0$, and write $\Delta\rho=\rho_m-\rho_c>0$. A positive added load depresses the plate, so $w$ is negative beneath it. Because bending moves the original surface while the load adds thickness, the final topography is **$e=s+w$**. For the cosine mode the horizontal biharmonic operator multiplies $w$ by $k^4$, giving

$$
(Dk^4+g\rho_m)w=-g\rho_cs.
$$

Eliminate $s=e-w$ to obtain

$$
\boxed{e=-\frac{Dk^4+g\Delta\rho}{g\rho_c}\,w.}
$$

The original loading equation contains $\rho_m$, whereas the relation after eliminating the added thickness contains $\Delta\rho$. These must not be interchanged prematurely.

At first order in the relief, represent a displaced [density](../../../../../density.md) interface by a sinusoidal mass sheet. A sheet of surface-density [amplitude](../../../../../wave-amplitude.md) $\Sigma$ at depth $z$ produces a downward gravity [amplitude](../../../../../wave-amplitude.md) $2\pi G\Sigma e^{-kz}$ at the datum. This follows by solving the Fourier-transformed gravitational [Poisson equation](../../../../../poisson-s-equation.md) above and below the sheet: the decaying potential has [amplitude](../../../../../wave-amplitude.md) $-2\pi G\Sigma e^{-k|z-z_0|}/k$, with the normal derivative jump fixed by the sheet mass.

The top interface contributes $\rho_ce$; the displaced [crust](../../../../../planetary-crust.md)–[mantle](../../../../../planetary-mantle.md) interface contributes $\Delta\rho\,w$ at depth $t$. Thus

$$
\Delta g=2\pi G[\rho_ce+\Delta\rho\,w e^{-kt}].
$$

The second term is negative beneath a positive load: depression replaces denser [mantle](../../../../../planetary-mantle.md) material by lighter [crust](../../../../../planetary-crust.md). Substituting the deflection-to-topography ratio yields

$$
\boxed{\Delta g=Z(k)e,\qquad
Z(k)=2\pi G\rho_c\left[1-
\frac{e^{-kt}}{1+Dk^4/(g\Delta\rho)}\right].}
$$

This [flexural gravity admittance](../../../../../flexural-gravity-admittance.md) combines mechanical compensation and attenuation of the buried interface's gravitational signal. It assumes small relief, a flat uniform thin plate, uniform [density](../../../../../density.md) layers and the stated surface loading, without additional internal [density](../../../../../density.md) anomalies. Here $t$ is the depth of the [crust](../../../../../planetary-crust.md)–[mantle](../../../../../planetary-mantle.md) interface. It is not automatically the [effective elastic thickness](../../../../../effective-elastic-thickness.md) $T_e$; the latter enters through $D=ET_e^3/[12(1-\nu^2)]$.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the physics of the Earth as a Planet course of the University of Cambridge](../../../../split.md)
6. [Physics of the Earth as a Planet course of the University of Cambridge](../../../../../physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)

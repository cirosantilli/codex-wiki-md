<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The finite angular resolution of [COBE DMR](../../../../differential-microwave-radiometer.md) suppresses small angular scales, so only low [spherical harmonic](../../../../spherical-harmonic.md) multipoles can be recovered usefully. The approximate relation $\theta\sim\pi/l$ associates $l\simeq17$ with scales of order ten degrees; this is an effective sensitivity and beam-window limit, not a mathematical hard truncation.

Interpret the printed superscript uncertainty as $(1.1\pm0.1)\times10^{-5}$. Its square estimates the band-limited zero-separation [variance](../../../../variance-split.md), rather than the full $C(0)$:

$$
\sigma_{2:17}^2=\frac{1}{4\pi}\sum_{l=2}^{17}(2l+1)C_l
=\frac{0.732\times4.43}{4\pi}\Delta_\phi^2.
$$

Use the coefficient supplied in the paper for this numerical inference. With $\sigma_{2:17}=1.1\times10^{-5}$,

$$
\Delta_\phi^2=4.69\times10^{-10},\qquad H_0=2.269\times10^{-18}\ \mathrm{s^{-1}},
$$

so [c](../c.md) gives

$$
\boxed{A=\frac{8\pi^2c^4\Delta_\phi^2}{9H_0^4}=1.25\times10^{96}\ \mathrm{m^4}=1.38\times10^6\ \mathrm{Mpc^4}.}
$$

The stated amplitude uncertainty gives approximately $18\%$ relative uncertainty in $A$, or $A\simeq(1.38\pm0.25)\times10^6\ \mathrm{Mpc^4}$, keeping $H_0$ fixed. The ideal matter-era [Sachs-Wolfe plateau](../../../../sachs-wolfe-plateau.md) with precisely the [c](../c.md) spectrum convention has coefficient $2\pi/9=0.698$, rather than $0.732$; the supplied numerical coefficient is about $5\%$ larger and has been treated as the paper's prescribed approximation. A real beam-convolved analysis retains its window function and additional cosmological transfer effects.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the astrophysics course of the University of Oxford](../../../split.md)
5. [Astrophysics course of the University of Oxford](../../../../astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**The printed line-density statement is incorrect for a phase-mixed [orbit](../../../../../../orbit-dynamical-system.md)**. A steady [line density on a Kepler orbit](../../../../../../line-density-on-a-kepler-orbit.md) is inversely proportional to speed: for a [cross-sectional-area current](../../../../../../cross-sectional-area-current.md) $J_\sigma$, the area per unit arc length is $d\sigma/ds=J_\sigma/v$. Equivalently, [phase mixing](../../../../../../phase-mixing.md) gives $d\sigma=(\sigma_{\rm tot}/P)\,dt$, uniform in [mean anomaly](../../../../../../mean-anomaly.md), where $P=2\pi\sqrt{a^3/\mu}$ is the [orbital period](../../../../../../orbital-period.md).

For an [optically thin](../../../../../../optically-thin-medium.md) population of [blackbodies](../../../../../../blackbody.md) in [radiative equilibrium](../../../../../../radiative-equilibrium.md), a fragment absorbs $\sigma L_\star/(4\pi r^2)$ and reradiates the same [luminosity](../../../../../../luminosity.md). Thus the [fractional luminosity of a phase-mixed eccentric wire](../../../../../../fractional-luminosity-of-a-phase-mixed-eccentric-wire.md) is

$$
f=\frac{\sigma_{\rm tot}}{4\pi P}\int_0^P\frac{dt}{r^2}.
$$

The [specific angular momentum](../../../../../../specific-angular-momentum.md) gives $dt/r^2=d\theta/h$, so the integral is $2\pi/h$. Since $Ph=2\pi a^2\sqrt{1-e^2}$,

$$
\boxed{f=\frac{\sigma_{\rm tot}}{4\pi a^2\sqrt{1-e^2}}}.
$$

This derives the intended result after explicitly correcting the density to $1/v$.

The error is consequential. If one instead imposes the literal density $d\sigma/ds\propto v$, its time weighting is $v^2dt$. Using $\langle v^2\rangle=\mu/a$, $\langle r^{-2}\rangle=[a^2\sqrt{1-e^2}]^{-1}$ and $\langle r^{-3}\rangle=[a^3(1-e^2)^{3/2}]^{-1}$ gives

$$
f_{\lambda_\ell\propto v}=\frac{\sigma_{\rm tot}}{4\pi a^2}\frac{1+e^2}{(1-e^2)^{3/2}}.
$$

At $e=1/2$ this is $5/3$ times the printed result. The inverse-radius averages can also be obtained directly with [eccentric anomaly](../../../../../../eccentric-anomaly.md) $E$, $r=a(1-e\cos E)$ and $dt=(1-e\cos E)dE/n$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 316](../../../paper-316-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

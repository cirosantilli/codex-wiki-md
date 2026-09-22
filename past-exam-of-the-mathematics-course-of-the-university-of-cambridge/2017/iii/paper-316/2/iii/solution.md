<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $A=\beta\mu/c$. The [Poynting–Robertson drag](../../../../../../poynting-robertson-drag.md) [acceleration](../../../../../../acceleration.md) has $\bar R=-2A\dot r/r^2$ and $\bar T=-A v_\theta/r^2$. Its [work](../../../../../../work.md) is strictly dissipative:

$$
\dot\varepsilon=-\frac A{r^2}(2\dot r^2+v_\theta^2).
$$

For an unperturbed [elliptic orbit](../../../../../../elliptic-orbit.md), use $dt=r^2df/h$, $\dot r=(\mu/h)e\sin f$ and $v_\theta=(\mu/h)(1+e\cos f)$. Averaging over its [orbital period](../../../../../../orbital-period.md) $P$ gives

$$
\langle\dot\varepsilon\rangle
=-\frac{A\mu^2}{Ph^3}\int_0^{2\pi}
[2e^2\sin^2f+(1+e\cos f)^2]\,df
=-\frac{A\mu^2\pi(2+3e^2)}{Ph^3}.
$$

Since $\dot a=2a^2\dot\varepsilon/\mu$, $P=2\pi a^{3/2}/\sqrt\mu$ and $h^3=\mu^{3/2}a^{3/2}(1-e^2)^{3/2}$, the [Poynting–Robertson decay of a circumstellar orbit](../../../../../../poynting-robertson-decay-of-a-circumstellar-orbit.md) is

$$
\boxed{\langle\dot a\rangle_{\rm cs}=-\frac{\beta\mu}{ca}
\frac{2+3e^2}{(1-e^2)^{3/2}}}.
$$

For a [circular Kepler orbit](../../../../../../circular-kepler-orbit.md) this becomes $-2A/a$. This is a secular first-order average, not an exact instantaneous decay law. If static [radiation pressure](../../../../../../radiation-pressure.md) is appreciable, use a bound conservative [orbit](../../../../../../orbit-dynamical-system.md) with central parameter $\mu_{\rm eff}=(1-\beta)\mu$, requiring $0\leq\beta<1$, and define its [orbital elements](../../../../../../orbital-element.md) accordingly; repeating the [work](../../../../../../work.md) calculation cancels $\mu_{\rm eff}$ and leaves the same coefficient $A=\beta GM_\star/c$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 316](../../../paper-316-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

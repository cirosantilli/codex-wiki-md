# Second virial coefficient

↑ **Parent:** [Virial expansion](virial-expansion.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Second_virial_coefficient)

The [second virial coefficient](second-virial-coefficient.md) is the leading interaction correction to the [ideal gas law](ideal-gas-law.md): at fixed [temperature](temperature.md), $B_2(T)=\lim_{n\to0}(Z-1)/n$, where $Z=p/(nk_BT)$ and $n$ is [number density](number-density.md). For identical classical particles in a homogeneous three-dimensional [gas](gas.md), with an isotropic [pair potential](pair-potential.md) $u(r)$ and $r$ the centre-to-centre separation,

$$
B_2(T)=-\frac12\int_{\mathbb R^3} f(|\mathbf r|)\,d^3\mathbf r
=2\pi\int_0^\infty\left[1-e^{-u(r)/(k_BT)}\right]r^2\,dr,
\qquad f(r)=e^{-u(r)/(k_BT)}-1.
$$

The function $f$ is the [Mayer f-function](mayer-f-function.md). The factor $4\pi r^2dr$ counts the [volume](volume.md) of a thin spherical shell; the factor $1/2$ counts each unordered pair once. The result has units of [volume](volume.md). Repulsive regions, $u>0$, contribute positively, while attractive regions, $u<0$, contribute negatively. [Tong, section 2.5.2, equations 2.75–2.76](https://davidtong.org/teaching/statistical-physics/statmechhtml/S2#S2.S5.SS2)

This is a striking bridge from a microscopic [pair potential](pair-potential.md) to a macroscopic [pressure](pressure.md) reading. At sufficiently small [number density](number-density.md), $B_2>0$ raises [pressure](pressure.md) relative to an [ideal gas](ideal-gas.md) at the same [temperature](temperature.md) and [number density](number-density.md), while $B_2<0$ lowers it. A single value of $B_2$, however, cannot determine the entire [pair potential](pair-potential.md): many different functions have the same weighted [integral](integral.md). Measurements over several [temperatures](temperature.md) supply more information.

The [integral](integral.md) must exist. For example, a bounded short-range attraction outside a hard core has no difficulty. If instead $u(r)\sim A/r^s$ as $r\to\infty$, then $1-e^{-u/(k_BT)}\sim u/(k_BT)$ and the radial tail behaves like $\int r^{2-s}dr$: it converges only for $s>3$. A bare unscreened [Coulomb potential](coulomb-potential-energy.md) therefore falls outside this formula's ordinary short-range setting. This condition on the tail does not by itself establish the stability or convergence of the full [virial expansion](virial-expansion.md).

For an exactly integrable toy attraction, choose the following square-well [pair potential](pair-potential.md), with diameter $\sigma>0$, attraction depth $\epsilon>0$, and range multiplier $a>1$:

$$
u(r)=\begin{cases}
+\infty,&0\le r<\sigma,\\
-\epsilon,&\sigma\le r<a\sigma,\\
0,&r\ge a\sigma.
\end{cases}
$$

Set $T^*=k_BT/\epsilon$ and $b_{\mathrm{HS}}=2\pi\sigma^3/3$, the [second virial coefficient](second-virial-coefficient.md) of a [hard-sphere gas](hard-sphere-gas.md). Integrating the core and attractive shell separately gives the exact toy result

$$
B_2(T)=b_{\mathrm{HS}}\left[1-(a^3-1)\left(e^{1/T^*}-1\right)\right].
$$

The core contributes $b_{\mathrm{HS}}$; the shell contributes $-b_{\mathrm{HS}}(a^3-1)(e^{1/T^*}-1)$. Heating weakens the relative [Boltzmann factor](boltzmann-factor.md) enhancement of attractive configurations, so $B_2$ approaches the positive hard-core value as $T^*\to\infty$. For the illustrative choice $a=3/2$, the zero occurs at

$$
T^*_0=\frac{1}{\log\left(1+\frac{1}{a^3-1}\right)}
=\frac{1}{\log(27/19)}\approx2.846.
$$

At this [temperature](temperature.md), $Z=1+B_3n^2+\cdots$: cancellation removes the linear correction, not every correction. At low $T^*$, the negative shell contribution becomes large, requiring a correspondingly smaller [number density](number-density.md) for a useful truncated [virial expansion](virial-expansion.md). The square well is a deliberately chosen model, not a fit to the [carbon dioxide](carbon-dioxide.md) experiment.

## ↑ Ancestors (5)

1. [Virial expansion](virial-expansion.md)
2. [Statistical physics](statistical-physics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Gas thermometer](gas-thermometer.md)
- [Hard-sphere gas](hard-sphere-gas.md)
- [Mayer f-function](mayer-f-function.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/35a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-355/3/b/solution.md)
- [Second virial coefficient](second-virial-coefficient.md)
- [Virial expansion](virial-expansion.md)

<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the two outer branches, $|u|\gg v_0$ at small $k$. An [integration by parts](../../../../integration-by-parts.md) and a large-$u$ expansion give

$$
I(u)=\int\frac{f_0(v)}{(v-u)^2}\,dv=\frac{n_*}{u^2}+O(u^{-3}),\qquad n_*=\int f_0(v)\,dv.
$$

There is no boundary contribution because the [phase-space distribution function](../../../../phase-space-distribution-function.md) vanishes at both endpoints. Direct area integration gives

$$
n_*=A_0\left[v_0+\delta\left(1-\frac{v_1}{v_0}\right)\right],\qquad \frac{n_*}{n_0}=1+\frac{\delta(v_0-v_1)}{v_0^2}.
$$

Thus the exact small-$k$ cutoff, retaining the paper's definition $n_0=v_0A_0$, is $\omega\to\pm\omega_{\mathrm{pe}}\sqrt{n_*/n_0}$. To leading order in the narrow-[velocity plateau](../../../../velocity-plateau.md) approximation this is

$$
\boxed{\omega\approx\pm\omega_{\mathrm{pe}}.}
$$

These are [Langmuir waves](../../../../langmuir-wave.md). The difference between $n_*$ and the reference $n_0$ is only first order in $\delta/v_0$, so it does not alter the requested leading-order result.

For the finite-[phase velocity](../../../../phase-velocity.md) branch put $u=v_1+\delta a$, with $0<a<1$. To leading order in $\delta/v_0$ and $\delta/v_1$, the real [dispersion relation](../../../../dispersion-relation-split.md) becomes

$$
\ln\left[\frac{v_1^2}{v_0^2-v_1^2}\frac{1-a}{a}\right]=K.
$$

At long wavelength set $K=0$ to leading order. Then $a=v_1^2/v_0^2$, and

$$
\boxed{\omega_{\mathrm a}\approx k\left[v_1+\delta\frac{v_1^2}{v_0^2}\right].}
$$

For comparison, the exact $k\to0$ [phase velocity](../../../../phase-velocity.md) from the [cubic equation](../../../../cubic-equation.md) in [b](../b.md) is $B/A$; expanding it gives precisely $v_1+\delta v_1^2/v_0^2+O(\delta^2/v_0)$ at fixed $v_1/v_0$.

A single [Maxwell-Boltzmann velocity distribution](../../../../maxwell-boltzmann-velocity-distribution.md) has a nonzero slope at every finite nonzero $u$ and has no [velocity plateau](../../../../velocity-plateau.md). The would-be [electron acoustic wave](../../../../electron-acoustic-wave.md) is therefore subject to strong [Landau damping](../../../../landau-damping.md), so there is no corresponding completely undamped acoustic branch in a single [Maxwellian](../../../../local-maxwellian.md) electron population with immobile ions. At its only stationary point $u=0$, a [Maxwellian](../../../../local-maxwellian.md) has $\int f_0'(v)/v\,dv<0$, making the static [dielectric function](../../../../dielectric-function.md) positive rather than zero. This statement does not exclude acoustic modes of suitably distinct electron populations or an ion-supported mode when ion dynamics is retained.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

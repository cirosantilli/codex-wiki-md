<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let the source's [hydrogen-ionizing photon production rate](../../../../../hydrogen-ionizing-photon-production-rate.md) be

$$
Q_{\rm H}=\int_{\nu_0}^{\infty}\frac{L_\nu}{h\nu}\,d\nu,
$$

where $h\nu_0$ is the hydrogen [ionization energy](../../../../../ionization-energy.md). The idealized [Strömgren sphere](../../../../../stromgren-sphere.md) has an almost fully ionized interior and a thin [ionization front](../../../../../ionization-front.md). In [photoionization equilibrium](../../../../../photoionization-equilibrium.md), every ionization is balanced by a [Case B recombination](../../../../../case-b-recombination.md), so spherical symmetry gives

$$
Q_{\rm H}=4\pi\int_0^{R_S}\alpha_B n_en_p r^2\,dr.
$$

For pure hydrogen of constant [number density](../../../../../number-density.md) $n$, the interior has $n_e=n_p=n$, and the [Strömgren radius](../../../../../stromgren-radius.md) is therefore

$$
\boxed{R_S=\left(\frac{3Q_{\rm H}}{4\pi\alpha_Bn^2}\right)^{1/3}}.
$$

Now let the effective number of dust grains per hydrogen nucleus be $f_d$, so the dust [absorption coefficient](../../../../../absorption-coefficient.md) is $a(r)=f_d\sigma_dn(r)$. If $Q(r)$ is the ionizing-photon rate crossing the sphere of radius $r$, recombinations and dust absorption give the [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation.md)

$$
\frac{dQ}{dr}+a(r)Q=-4\pi r^2\alpha_Bn(r)^2,
\qquad Q(0)=Q_{\rm H},\qquad Q(R_d)=0.
$$

If $f_d$ denotes a dust mass fraction instead, the grain mass and gas mean particle mass are simply absorbed into the effective product $f_d\sigma_d$. Define the [dust optical depth](../../../../../dust-optical-depth.md)

$$
\tau_d(r)=\int_0^r f_d\sigma_dn(s)\,ds.
$$

Multiplication by the [integrating factor](../../../../../integrating-factor.md) $e^{\tau_d(r)}$ and integration to the dusty front gives its governing equation

$$
\boxed{Q_{\rm H}=4\pi\alpha_B\int_0^{R_d}n(r)^2r^2e^{\tau_d(r)}\,dr}.
$$

The [exponential function](../../../../../exponential-function.md) weights recombinations at large optical depth by the extra source photons that dust must remove before those photons reach that radius.

For constant $n$, put $a=f_d\sigma_dn$ and $\tau=aR_d$. The elementary [integral](../../../../../integral.md)

$$
\int_0^{R_d}r^2e^{ar}\,dr
=\frac{e^\tau(\tau^2-2\tau+2)-2}{a^3}
$$

reduces the equation to

$$
\boxed{Q_{\rm H}=\frac{4\pi\alpha_Bn^2}{a^3}
\left[e^\tau(\tau^2-2\tau+2)-2\right]}.
$$

Equivalently, with $y=R_d/R_S$ and $\tau_S=aR_S$,

$$
\boxed{e^{\tau_Sy}\left[(\tau_Sy)^2-2\tau_Sy+2\right]-2=\frac{\tau_S^3}{3}}.
$$

Its dust-free [limit](../../../../../limit-of-a-function.md) is $y\to1$, while absorption makes $R_d\lt R_S$ for nonzero dust abundance.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 349](../../paper-349-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

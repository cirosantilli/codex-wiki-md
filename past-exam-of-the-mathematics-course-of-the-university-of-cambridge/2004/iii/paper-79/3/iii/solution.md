<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the quadratic spectral flux $S_z=-\tfrac12\operatorname{Re}(V^*T)$. For positive real material [mass density](../../../../../../density.md) and [shear modulus](../../../../../../shear-modulus.md), differentiation of the [velocity](../../../../../../velocity.md)–[traction](../../../../../../traction.md) system gives

$$
S_z'=-\frac12\operatorname{Re}\left[\frac{i\omega^*}{\mu}|T|^2-i\omega\mu p_\beta^2|V|^2\right].
$$

Because $k$ is real, $\mu p_\beta^2=\rho-\mu k^2/\omega^2$. If $v=\operatorname{Im}\omega>0$, then $\operatorname{Re}(i\omega^*)=v$ and $\operatorname{Re}(-i\omega\mu p_\beta^2)=v(\rho+\mu k^2/|\omega|^2)$. This proves [complex-frequency SH flux monotonicity](../../../../../../complex-frequency-sh-flux-monotonicity.md):

$$
\boxed{S_z'=-\frac v2\left[\frac{|T|^2}{\mu}
+\left(\rho+\frac{\mu k^2}{|\omega|^2}\right)|V|^2\right]<0.}
$$

Strictness holds for a nontrivial wavefield: if $V,T$ vanished together at one point, uniqueness of the first-order system would make the entire solution zero. The zero solution is the necessary exception to the literal strict inequality. Across a bonded material boundary $V,T$, and hence $S_z$, are continuous; integrating the negative [derivative](../../../../../../derivative.md) gives strict decrease across any positive-depth interval as well.

Where the [SH input impedance](../../../../../../sh-input-impedance.md) is finite, $S_z=\tfrac12\operatorname{Re}Z|V|^2$. If $\operatorname{Re}Z(z_1)>0$, then $S_z(z_1)>0$ and all shallower fluxes are larger and positive. They cannot have $V=0$, since that would make $S_z=0$. Thus **$\operatorname{Re}Z(z)>0$ for every $z<z_1$**. Likewise, negative real [SH input impedance](../../../../../../sh-input-impedance.md) at $z_0$ gives negative flux throughout $z>z_0$, excludes [velocity](../../../../../../velocity.md) zeros there and implies **$\operatorname{Re}Z(z)<0$ for every $z>z_0$**.

In a uniform region let $q=\mu p_\beta$ on the [causal vertical wavenumber branch](../../../../../../causal-vertical-wavenumber-branch.md). The constant Riccati solutions are $Z=\pm q$, and integrating the one-way equation gives

$$
\boxed{V(z)\propto e^{\pm i\omega p_\beta z}=e^{\pm ik_\beta z}.}
$$

Since $\operatorname{Re}q>0$, the plus solution carries positive downward flux and the minus solution negative upward flux. Writing $k_\beta=a+ib$ with $b>0$, their moduli are proportional to $e^{-bz}$ and $e^{bz}$ respectively: each decays in its direction of [energy](../../../../../../energy.md) flow.

For complex [frequency](../../../../../../frequency.md) the displayed quadratic form is the spectral flux diagnostic specified in the question; a genuinely periodic time average is recovered on the real-frequency axis. The decrease here comes from the upper-half-plane convergence parameter, not from material dissipation. At real [frequency](../../../../../../frequency.md) in a lossless layer the corresponding flux is constant.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

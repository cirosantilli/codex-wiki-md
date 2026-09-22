<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

In the radiative layer, take the enclosed [mass](../../../../../mass.md) to be $M_1$, the transported [luminosity](../../../../../luminosity.md) to be $L$, and the [mean molecular weight](../../../../../mean-molecular-weight.md) to be constant. The envelope's own gravity is neglected. Divide the hydrostatic and radiative [temperature](../../../../../temperature.md) equations, and then eliminate density using the gas equation of state:

$$
\frac{dP}{dT}=\frac{16\pi acGM_1}{3\kappa L}T^3
=B\frac{T^{3+m+n}}{P^n},\qquad
B=\frac{16\pi acGM_1}{3\kappa_0L}\left(\frac{\mathcal R}{\mu}\right)^n.
$$

Put $p=n+1$ and $b=4+m+n$. For $p,b\ne0$, integration gives

$$
P^p=\frac{pB}{b}T^b+K_P.
$$

Defining $C^p=pB/b$ and $K=K_P/C^p$ yields

$$
\boxed{P=C(T^b+K)^{1/p},\qquad
C=\left[\frac{16\pi acGM_1}{3\kappa_0L}
\left(\frac{\mathcal R}{\mu}\right)^n\frac{n+1}{4+m+n}\right]^{1/(n+1)}.}
$$

In the relevant positive-exponent case, writing $K=T_0^b$ produces the stated form whenever this integration constant is nonnegative. The exceptional values excluded above lead to logarithms: $p=0$ gives $\log P=BT^b/b+\mathrm{const}$, $b=0$ gives $P^p=pB\log T+\mathrm{const}$, and both zero give $\log P=B\log T+\mathrm{const}$.

For [radiative-envelope convection matching](../../../../../radiative-envelope-convection-matching.md), compute the logarithmic gradient of the [pressure](../../../../../pressure.md) relation:

$$
\nabla_{\mathrm{rad}}=\frac{d\log T}{d\log P}
=\frac pb\left(1+\frac K{T^b}\right).
$$

At the marginal boundary, the [Schwarzschild criterion](../../../../../schwarzschild-criterion.md) equates this with the ideal-gas adiabatic gradient $\nabla_{\mathrm{ad}}=(\gamma-1)/\gamma$. Hence

$$
K=T_b^b\left[\frac bp\frac{\gamma-1}{\gamma}-1\right],
\qquad
\boxed{T_0=T_b\left[\frac{\gamma-1}{\gamma}
\frac{4+m+n}{n+1}-1\right]^{1/(4+m+n)}.}
$$

The positive real $T_0$ notation requires a nonnegative bracket; a general signed $K$ is the safer integration constant otherwise. For the later case $n=1,m=3$ and a monatomic gas, this bracket is $3/5$, so $T_0$ is of the same order as $T_b$.

Deep below the convective boundary, with the temperature-power term dominating $K$, the [pressure](../../../../../pressure.md) law becomes $P\simeq CT^{b/p}$. Differentiating this approximation and using hydrostatic balance gives

$$
\frac bp\frac PT\frac{dT}{dr}
=-\frac{GM_1}{r^2}\frac{\mu P}{\mathcal RT},
\qquad
\frac{dT}{dr}=-\frac{\mu GM_1p}{\mathcal Rb}\frac1{r^2}.
$$

The general [temperature](../../../../../temperature.md) is a term proportional to $1/r$ plus a boundary-dependent constant. Well inside the boundary radius, where that term dominates, it reduces to

$$
\boxed{T(r)\simeq\frac{\mu GM_1(n+1)}{\mathcal R(4+m+n)r}.}
$$

The inverse-radius profile is an inner approximation, not an assertion that the boundary term vanishes everywhere.

Now take $n=1,m=3$, so $p=2$, $b=8$. Then $P\simeq CT^4$, $\rho\simeq(\mu C/\mathcal R)T^3$, and define $A_T=\mu GM_1/(4\mathcal R)$ so that $T\simeq A_T/r$. The [luminosity](../../../../../luminosity.md) supplied by the thin burning layer is

$$
\begin{aligned}
L&\simeq4\pi\int_{R_1}^{r_b}r^2\rho\epsilon\,dr
=4\pi C^2\epsilon_0\left(\frac\mu{\mathcal R}\right)^2
A_T^{16}\int_{R_1}^{r_b}r^{-14}\,dr\\
&=\frac{4\pi}{13}C^2\epsilon_0\left(\frac\mu{\mathcal R}\right)^2
A_T^{16}(R_1^{-13}-r_b^{-13}).
\end{aligned}
$$

Because the integral is strongly concentrated near $R_1$ and $r_b\gg R_1$, the outer term is negligible. Thus

$$
\boxed{L\simeq\frac{4\pi}{13}C^2\epsilon_0
\left(\frac\mu{\mathcal R}\right)^2
\left(\frac{\mu GM_1}{4\mathcal R}\right)^{16}\frac1{R_1^{13}}.}
$$

The factor $\rho\epsilon$, rather than merely $\epsilon$, is essential since the specified energy-generation rate is per unit [mass](../../../../../mass.md). This integration uses the deep radiative profile as a leading thin-shell approximation.

Crucially, $C$ is not independent of [luminosity](../../../../../luminosity.md). Its defining relation gives

$$
C^2=\frac{4\pi acGM_1}{3\kappa_0L}\frac{\mathcal R}{\mu}
\propto\frac{M_1}{L}.
$$

Substitution into the shell integral therefore yields $L^2\propto M_1^{17}R_1^{-13}$. The degenerate-core relation gives $R_1\propto M_1^{-1/3}$, so

$$
L^2\propto M_1^{17+13/3}=M_1^{64/3},\qquad
\boxed{L\propto M_1^{32/3}.}
$$

This [degenerate-core shell-burning mass-luminosity relation](../../../../../degenerate-core-shell-burning-mass-luminosity-relation.md) is specific to the adopted [opacity](../../../../../opacity.md), burning exponent and structural approximations.

Removing some envelope [mass](../../../../../mass.md) while retaining the hydrogen-burning shell and the deep-envelope regime leaves the leading [luminosity](../../../../../luminosity.md) approximately unchanged at fixed core [mass](../../../../../mass.md). The envelope can instead change the radius and [effective temperature](../../../../../effective-temperature.md). This independence is not valid for arbitrarily complete stripping: removing the fuel or the pressure-confined shell structure quenches or modifies shell burning, and the assumed giant model then fails.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

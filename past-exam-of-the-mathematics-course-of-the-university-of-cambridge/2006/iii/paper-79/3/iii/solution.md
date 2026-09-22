<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Combining the [Kolmogorov two-thirds law](../../../../../../kolmogorov-two-thirds-law.md) with the [Kolmogorov four-fifths law](../../../../../../kolmogorov-four-fifths-law.md) gives the [velocity increment](../../../../../../velocity-increment.md) [skewness](../../../../../../skewness.md) in the [inertial range](../../../../../../inertial-range.md):

$$
S(r)=\frac{S_3(r)}{S_2(r)^{3/2}}
=\frac{-4\epsilon r/5}{[\beta(\epsilon r)^{2/3}]^{3/2}}
=\boxed{-\frac4{5\beta^{3/2}}}.
$$

The [constant-skewness turbulence closure](../../../../../../constant-skewness-turbulence-closure.md) assumes this same value throughout the [universal equilibrium range](../../../../../../equilibrium-range.md), including the dissipative crossover. This is an extra modeling assumption; neither similarity law establishes it near $r=0$.

Write $A=\beta(15\beta)^{1/2}$, $B=(15\beta)^{3/4}$, $S_2=Av^2h$ and $r=B\eta x$. Since $\nu=v\eta$ and $\epsilon\eta=v^3$, substituting $S_3=-4S_2^{3/2}/(5\beta^{3/2})$ into the [Kolmogorov equation for structure functions](../../../../../../kolmogorov-equation-for-structure-functions.md) gives

$$
\frac{6A}{B}h'+\frac{4A^{3/2}}{5\beta^{3/2}}h^{3/2}=\frac45Bx.
$$

Dividing by $2B/5$ yields the [normalized constant-skewness structure-function equation](../../../../../../normalized-constant-skewness-structure-function-equation.md):

$$
\boxed{\frac{dh}{dx}+2h^{3/2}=2x,\qquad h(0)=0}.
$$

At small $x$, $h\sim x^2$, recovering $S_2\sim\epsilon r^2/(15\nu)$ for differentiable [velocity increments](../../../../../../velocity-increment.md). At large $x$, the dominant balance gives $h\sim x^{2/3}$, recovering the assumed [Kolmogorov two-thirds law](../../../../../../kolmogorov-two-thirds-law.md).

This [turbulence closure](../../../../../../turbulence-closure.md) is inexpensive: a single [ordinary differential equation](../../../../../../ordinary-differential-equation.md) interpolates between the two regimes while respecting the local third-order balance. Its prescribed [skewness](../../../../../../skewness.md) cannot independently predict scale-dependent derivative statistics, transient spectral evolution or [internal intermittency](../../../../../../internal-intermittency.md).

[EDQNM closure](../../../../../../eddy-damped-quasi-normal-markovian-closure.md) instead evolves the [turbulent energy spectrum](../../../../../../turbulent-energy-spectrum.md) through modeled [spectral triad interactions](../../../../../../spectral-triad-interaction.md). Its quasi-normal fourth-order approximation is supplemented by eddy damping and a Markovian treatment of correlation memory. It retains more information about scale-dependent transfer and evolving spectra, at the cost of spectral integrals and modeled damping times. It is still approximate and does not automatically describe coherent structures or [internal intermittency](../../../../../../internal-intermittency.md). The simple constant-skewness model is therefore useful as an equilibrium interpolation; [EDQNM closure](../../../../../../eddy-damped-quasi-normal-markovian-closure.md) addresses a broader spectral evolution problem.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

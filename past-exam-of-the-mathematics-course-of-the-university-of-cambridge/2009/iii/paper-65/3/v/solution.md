<h1 id="3/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

First specify the dynamical estimate: assume an initially isolated virialized system, stars of different [masses](../../../../../../mass.md) well mixed with the same velocity distribution, and ejecta escaping rapidly compared with a [stellar crossing time](../../../../../../stellar-crossing-time.md), without imparting kicks to surviving stars. If $f$ is the retained stellar [mass](../../../../../../mass.md) fraction, the original [virial theorem](../../../../../../virial-theorem.md) gives $2T+W=0$, where $T$ is [kinetic energy](../../../../../../kinetic-energy.md) and $W<0$ is [Newtonian gravitational potential energy](../../../../../../newtonian-gravitational-potential-energy.md). Immediately after loss, positions and velocities are unchanged, so

$$
T'=fT,\qquad W'=f^2W,\qquad
E'=fT+f^2W=|W|f\left(\frac12-f\right).
$$

Thus [impulsive disruption by stellar mass loss](../../../../../../impulsive-disruption-by-stellar-mass-loss.md) makes the energy of the whole remaining system nonnegative when at least half the initial [mass](../../../../../../mass.md) is removed.

For the power-law [initial mass function](../../../../../../initial-mass-function.md), the fraction removed is a mass fraction, not a number fraction:

$$
F(\alpha)=\frac{\int_{10}^{100}x^{1-\alpha}dx}{\int_{0.1}^{100}x^{1-\alpha}dx}
=\frac{100^{2-\alpha}-10^{2-\alpha}}{100^{2-\alpha}-0.1^{2-\alpha}}
\quad(\alpha\ne2),\qquad F(2)=\frac{\ln10}{\ln1000}=\frac13.
$$

For integer slopes, $F(0)\simeq0.990$, $F(1)\simeq0.901$, $F(2)=0.333$, and $F(3)\simeq0.009$. Interpolating between $\alpha=1$ and $2$ puts the threshold around $1.7$--$1.8$. Solving $F=1/2$ more accurately gives

$$
2\,10^{2-\alpha}=100^{2-\alpha}+0.1^{2-\alpha},\qquad
\boxed{\alpha_{\rm crit}\simeq1.7910.}
$$

The rearranged equation has a spurious root at $\alpha=2$ introduced when the vanishing denominator was cleared; the logarithmic limit $F(2)=1/3$ excludes it. Increasing $\alpha$ shifts the mass distribution towards lower [masses](../../../../../../mass.md), so **the top-heavy side, $\alpha<\alpha_{\rm crit}$, has nonnegative remnant energy in the impulsive model**; equality is marginal. One can see strict monotonicity from the [covariance](../../../../../../covariance.md) obtained by differentiating $F$: $F'=-\operatorname{Cov}(\mathbf1_{x>10},\ln x)<0$ under the normalized mass-weighted distribution.

The [initial mass function](../../../../../../initial-mass-function.md) alone does not guarantee complete disruption. If losses occur slowly, the [adiabatic mass-loss expansion law](../../../../../../adiabatic-mass-loss-expansion-law.md) gives expansion rather than the instantaneous half-mass threshold, and positive total energy can still leave a bound core after selective escape. The stated value is therefore the conventional global impulsive estimate, with no external confining [Newtonian gravitational potential](../../../../../../newtonian-gravitational-potential.md).

## ↑ Ancestors (11)

1. [V](../v.md)
2. [3](../../3.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

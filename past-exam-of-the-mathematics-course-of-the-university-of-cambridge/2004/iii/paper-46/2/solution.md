<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use $\beta_{\rm th}=1/(k_BT)$ for inverse temperature to distinguish it from the order-parameter exponent. The decaying [two-point correlation function](../../../../../two-point-correlation-function.md) needed for the response identity is connected:

$$
G(r)=\langle\sigma_0\sigma_r\rangle-\langle\sigma_0\rangle\langle\sigma_r\rangle.
$$

Away from the critical point in a short-range [Ising model](../../../../../ising-model.md) pure phase, the [correlation length](../../../../../correlation-length.md) controls the exponential long-distance falloff, $G(r)\sim A(r)e^{-|r|/\xi}$ with a possible algebraic prefactor. The full two-spin expectation below the transition instead tends to $M^2$. The [spin-mixture contribution to zero-field susceptibility](../../../../../spin-mixture-contribution-to-zero-field-susceptibility.md) explains why a symmetric mixture is unsuitable for defining a finite connected correlation length in the ordered phase.

Let $F=-\beta_{\rm th}^{-1}\log Z$ be the total [Helmholtz free energy](../../../../../helmholtz-free-energy.md). Take magnetization and susceptibility per site, so

$$
M=-\frac1N F_h=\frac1N\left\langle\sum_r\sigma_r\right\rangle,\qquad
\chi=\frac{\partial M}{\partial h}=-\frac1NF_{hh}.
$$

Differentiating the [Boltzmann weights](../../../../../boltzmann-factor.md) at fixed temperature gives

$$
\chi=\frac{\beta_{\rm th}}N\left[\left\langle\left(\sum_r\sigma_r\right)^2\right\rangle-\left\langle\sum_r\sigma_r\right\rangle^2\right]
=\frac{\beta_{\rm th}}N\sum_{r,s}\langle\sigma_r\sigma_s\rangle_c.
$$

Translation invariance then yields the [correlation-function susceptibility sum rule](../../../../../correlation-function-susceptibility-sum-rule.md)

$$
\boxed{\chi=\beta_{\rm th}\sum_rG(r).}
$$

Total magnetization and total susceptibility multiply these expressions by $N$; per physical volume they have an additional factor $a^{-D}$ relative to the per-site convention. These normalizations do not change the critical powers.

For the subsequent scaling requests, let $F_s$ denote singular [free energy](../../../../../thermodynamic-free-energy.md) per site; the fixed extensive normalization is suppressed. The labels $+$ and $-$ denote $t>0$ and $t<0$, with distinct scaling functions and amplitudes on the two sides. Below the transition a one-sided derivative at $h=0$ selects a spontaneous-magnetization branch. Writing $x=h/|t|^\Delta$, differentiation of the [scaling hypothesis for critical phenomena](../../../../../scaling-hypothesis-for-critical-phenomena.md) gives

$$
M_s=-|t|^{2-\alpha-\Delta}f_\pm'(x),\qquad
\chi_s=-|t|^{2-\alpha-2\Delta}f_\pm''(x).
$$

The field-independent $I_\pm$ makes no contribution to these field derivatives, although it can change heat-capacity amplitudes. Assuming nonzero leading amplitudes and the indicated pure-phase limits, comparison with the exponent definitions gives

$$
\beta=2-\alpha-\Delta,\qquad \gamma=2\Delta+\alpha-2,
\qquad \boxed{\alpha+2\beta+\gamma=2.}
$$

This is the [Rushbrooke scaling relation](../../../../../rushbrooke-scaling-relation.md). A temperature-independent critical isotherm requires the large-$|x|$ magnetization scaling function to grow as $\operatorname{sgn}(x)|x|^{\beta/\Delta}$: otherwise $M_s=|t|^\beta\mathcal M_\pm(x)$ would retain a temperature power as $t\to0$ at fixed small $h$. Therefore $1/\delta=\beta/\Delta$. Since the preceding two equalities also give $\Delta=\beta+\gamma$, the [Widom scaling relation](../../../../../widom-scaling-relation.md) follows:

$$
\boxed{\beta\delta=\beta+\gamma.}
$$

For the [hyperscaling relation](../../../../../hyperscaling-relation.md), additionally assume that one [correlation volume](../../../../../correlation-volume.md) supplies an order-one singular free-energy contribution and that there is a single isotropic correlation length, with no [dangerously irrelevant coupling](../../../../../dangerously-irrelevant-coupling.md) spoiling this argument. Then $F_s\sim\xi^{-D}\sim|t|^{D\nu}$. Two temperature derivatives give the singular heat capacity, so

$$
\boxed{2-\alpha=D\nu.}
$$

Hyperscaling is an additional physical assumption, not a consequence of the two-variable equation alone, and generally fails above the [upper critical dimension](../../../../../upper-critical-dimension.md).

Finally the correlation scaling function $f_G(x)$ falls exponentially, up to algebraic factors, for $x\to\infty$ in a massive short-range pure phase. At $x\to0$ it approaches a finite nonzero value in the scaling regime. Approximating the lattice sum at distances much larger than $a$, and denoting the area of the unit sphere by $S_{D-1}$, gives

$$
\chi_s\simeq\frac{\beta_{\rm th}S_{D-1}}{a^D}\int_a^\infty r^{1-\eta}f_G(r/\xi)dr
=\frac{\beta_{\rm th}S_{D-1}}{a^D}\xi^{2-\eta}\int_{a/\xi}^\infty x^{1-\eta}f_G(x)dx.
$$

If $\eta<2$ and the integral has a finite nonzero limiting value, microscopic distances contribute only a regular background and the leading divergence is $\xi^{2-\eta}$. Thus the [Fisher scaling relation](../../../../../fisher-scaling-relation.md) is

$$
\boxed{\gamma=(2-\eta)\nu.}
$$

These statements concern leading singular powers; logarithmic corrections and cancellations of amplitudes require separate treatment.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

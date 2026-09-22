<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Use $S_C(r)=\langle(C'-C)^2\rangle$ for the [scalar structure function](../../../../../../scalar-structure-function.md), and assume [statistical homogeneity](../../../../../../statistical-homogeneity.md) as well as isotropy. Expanding the square gives

$$
S_C(r)=2\langle C^2\rangle-2\langle CC'\rangle.
$$

If the zero-mean scalar decorrelates at large separation, then

$$
\boxed{S_C(r)\longrightarrow2\langle C^2\rangle.}
$$

The decorrelation assumption is necessary: a spatially constant, zero-ensemble-mean random scalar is isotropic but has $S_C=0$ at every separation.

For the small-separation limit assume mean-square differentiability. Taylor expansion gives $C'-C=r_i\partial_iC+o(r)$ in mean square. Isotropy implies $\langle\partial_iC\partial_jC\rangle=\delta_{ij}\langle|\nabla C|^2\rangle/3$. Define the [scalar dissipation rate](../../../../../../scalar-dissipation-rate.md) in the half-variance convention, $\epsilon_c=\alpha\langle|\nabla C|^2\rangle$, so that [diffusion](../../../../../../diffusion.md) removes $\langle C^2/2\rangle$ at rate $\epsilon_c$. It follows that

$$
\boxed{S_C(r)=\frac{\epsilon_c}{3\alpha}r^2+o(r^2).}
$$

If dissipation is instead defined as the loss rate of the full [variance](../../../../../../variance-split.md), the coefficient must be adjusted by a factor of two.

In the [inertial-convective scalar range](../../../../../../inertial-convective-scalar-range.md), $\max(\eta,\eta_c)\ll r\ll\ell$, suppose [scalar variance](../../../../../../scalar-variance.md) cascades locally at an approximately constant flux $\epsilon_c$, while [velocity](../../../../../../velocity.md) increments have the [Kolmogorov 1941 theory](../../../../../../kolmogorov-1941-theory.md) turnover time $t_r\sim\epsilon^{-1/3}r^{2/3}$. The [variance](../../../../../../variance-split.md) associated with scale $r$ divided by that turnover time is of order its transfer rate, giving the [Obukhov-Corrsin theory](../../../../../../obukhov-corrsin-theory.md) result

$$
\boxed{S_C(r)\sim\epsilon_ct_r\sim\epsilon_c\epsilon^{-1/3}r^{2/3}.}
$$

The assumptions include a passive scalar, high Reynolds number, local transfer, adequate scale separation, and statistical equilibrium or sufficiently slow variation of the supply. Isotropy alone does not provide a constant scalar flux.

For weak scalar [diffusion](../../../../../../diffusion.md), $\alpha\ll\nu$, the [velocity](../../../../../../velocity.md) is smooth below $\eta$, with characteristic strain rate $s\sim(\epsilon/\nu)^{1/2}$. [Diffusion](../../../../../../diffusion.md) rate $\alpha/r^2$ balances this at the [Batchelor scalar microscale](../../../../../../batchelor-scalar-microscale.md)

$$
\eta_c=\eta_B\sim(\alpha/s)^{1/2}=(\alpha^2\nu/\epsilon)^{1/4}.
$$

In the [viscous-convective scalar range](../../../../../../viscous-convective-scalar-range.md), the derivative of $S_C$ is assumed to depend only on $\epsilon_c$, $s$ and $r$. Their dimensions force

$$
\frac{dS_C}{dr}\sim\frac{\epsilon_c}{sr}.
$$

Integration from the [diffusion](../../../../../../diffusion.md) cutoff gives

$$
S_C(r)=S_C(\eta_c)+A_B\frac{\epsilon_c}{s}\ln\left(\frac r{\eta_c}\right).
$$

Thus, well within a broad logarithmic range,

$$
\boxed{S_C(r)\sim\epsilon_c\sqrt{\frac\nu\epsilon}\ln(r/\eta_c).}
$$

The additive matching contribution is not exactly zero; the formula is a leading range estimate, not a boundary condition at $r=\eta_c$. Using $dS_C/dr$ isolates the contribution acquired on changing separation. The structure function itself contains [scalar variance](../../../../../../scalar-variance.md) accumulated from smaller scales and must retain the inner cutoff through its integration constant. If one assumed that $S_C$ depended only on $\epsilon_c,s,r$ without that cutoff, [dimensional analysis](../../../../../../dimensional-analysis.md) would incorrectly give an $r$-independent value proportional to $\epsilon_c/s$. This explains the use of the derivative with respect to $r$; the TeX aid changes that derivative to $t$ in its final sentence, but the original PDF consistently uses $r$.

Finally let $\alpha\gg\nu$. Balancing [diffusion](../../../../../../diffusion.md) with the inertial eddy rate gives the [Corrsin scalar microscale](../../../../../../corrsin-scalar-microscale.md) $\eta_c=\eta_C\sim(\alpha^3/\epsilon)^{1/4}\gg\eta$. For $\eta\ll r\ll\eta_c$, [diffusion](../../../../../../diffusion.md) is faster than the eddy turnover rate. The scalar is smooth to leading order on those separations, even though the [velocity](../../../../../../velocity.md) still has inertial-range fluctuations. The [inertial-diffusive scalar range](../../../../../../inertial-diffusive-scalar-range.md) therefore has

$$
\boxed{S_C(r)\simeq\frac{\epsilon_c}{3\alpha}r^2,\qquad\eta\ll r\ll\eta_c.}
$$

This continues the scalar's leading gradient-controlled quadratic behaviour; it is not a continuation of the inertial-convective two-thirds law below its [diffusion](../../../../../../diffusion.md) cutoff.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 87](../../../paper-87-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

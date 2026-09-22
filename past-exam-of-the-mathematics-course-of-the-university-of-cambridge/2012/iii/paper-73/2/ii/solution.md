<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [Landau intermittency counterexample](../../../../../../landau-intermittency-counterexample.md), combine two locally homogeneous turbulent populations, with the same sufficiently wide inertial interval but different [viscous dissipation](../../../../../../viscous-dissipation.md) rates $\epsilon_1$ and $\epsilon_2$. This can mean an ensemble randomly selected between two intensities, or large turbulent patches whose small-scale increments are sampled away from the patch boundaries. Suppose each population individually obeys the proposed universal coefficient $\beta_p$. If their proportions are $w$ and $1-w$, the combined [longitudinal structure function](../../../../../../longitudinal-velocity-structure-function.md) is

$$
S_p(r)=\beta_pr^{p/3}\left[w\epsilon_1^{p/3}+(1-w)\epsilon_2^{p/3}\right],\qquad
\epsilon=w\epsilon_1+(1-w)\epsilon_2.
$$

Its effective coefficient referenced to the global mean [viscous dissipation](../../../../../../viscous-dissipation.md) is therefore

$$
\boxed{\beta_p^{\rm eff}=\beta_p\frac{w\epsilon_1^{p/3}+(1-w)\epsilon_2^{p/3}}
{[w\epsilon_1+(1-w)\epsilon_2]^{p/3}}}.
$$

For a concrete example let $w=1/2$ and $\epsilon_{1,2}=\epsilon(1\pm d)$, with $0<d<1$. Then

$$
\frac{\beta_p^{\rm eff}}{\beta_p}=\frac{(1+d)^{p/3}+(1-d)^{p/3}}2.
$$

For $p=6$ this is $1+d^2$, explicitly dependent on the strength of the large-scale modulation. For $p=2$ it is less than one by concavity. Thus **coefficients based solely on mean [viscous dissipation](../../../../../../viscous-dissipation.md) cannot be universal under arbitrary [integral-scale intermittency](../../../../../../integral-scale-intermittency.md)**. The common inertial interval can be maintained by taking both local [Reynolds numbers](../../../../../../reynolds-number.md) sufficiently large.

At $p=3$ the ratio is exactly one. This exception is consistent with the signed third-order energy-flux law and must not be used to rescue universality of all other orders. For noninteger orders one uses absolute increments; the even-order examples already establish the counterexample without a sign convention ambiguity. The issue is the difference between a [moment](../../../../../../moment.md) of the local [viscous dissipation](../../../../../../viscous-dissipation.md) and the same power of its mean, not a failure of averaging itself.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

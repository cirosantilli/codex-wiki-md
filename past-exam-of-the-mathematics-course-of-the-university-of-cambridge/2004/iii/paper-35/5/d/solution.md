<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The unit [zero-coupon bond](../../../../../../zero-coupon-bond.md) pays one at maturity. Its [risk-neutral valuation](../../../../../../risk-neutral-pricing.md) therefore is

$$
\boxed{P(t,T)=\mathbb E_{\mathbb Q}\left[\exp\left(-\int_t^Tr_sds\right)\mid r_t=r\right].}
$$

No particular rate coefficients were specified, so this expectation is the general answer; evaluating it further requires a chosen [one-factor short-rate model](../../../../../../one-factor-short-rate-model.md).

For the alternative derivation let $D_t=\exp(-\int_0^tr_sds)$ be the bank [discount factor](../../../../../../discount-factor.md). For an integrable discounted payoff, pricing gives

$$
D_tV(t,r_t)=\mathbb E_{\mathbb Q}[D_TX\mid\mathcal F_t],
$$

which is a [martingale](../../../../../../martingale-split.md) by the [tower property of conditional expectation](../../../../../../law-of-total-expectation.md). For a payoff determined by the [Markov](../../../../../../markov-property.md) rate state, this conditional expectation is represented by the indicated pricing function. A path-dependent claim requires an appropriately enlarged state, as in part (c). Now $dD_t=-r_tD_tdt$ has finite variation. Applying [Itô formula](../../../../../../ito-s-lemma.md) and the product rule under the [risk-neutral measure](../../../../../../risk-neutral-measure.md), whose rate drift is $b-\sigma\theta$, yields

$$
d(D_tV)=D_t\left[V_t+(b-\sigma\theta)V_r+\frac12\sigma^2V_{rr}-rV\right]dt+D_t\sigma V_r\,d\widetilde W_t.
$$

Under the smoothness and integrability conditions used above, the [martingale](../../../../../../martingale-split.md) has zero finite-variation drift. The bracket therefore vanishes, giving again

$$
\boxed{V_t+(b-\sigma\theta)V_r+\frac12\sigma^2V_{rr}-rV=0.}
$$

For the bond the terminal condition is $P(T,T)=1$. This argument also shows why stochastic discounting remains inside the conditional expectation.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

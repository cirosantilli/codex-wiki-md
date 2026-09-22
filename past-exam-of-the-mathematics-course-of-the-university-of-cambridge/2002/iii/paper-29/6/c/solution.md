<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $D_s=\exp(-\int_0^sR_u\,du)$, where $R_u=F_{u,u}$ is the [short rate](../../../../../../short-rate.md). At maturity the [zero-coupon bond](../../../../../../zero-coupon-bond.md) pays one, so $Z_{T,T}=D_T$. If the discounted bond price is a [martingale](../../../../../../martingale-split.md), its terminal [conditional expectation](../../../../../../conditional-expectation.md) is

$$
D_sP_{s,T}=Z_{s,T}=\mathbb E[D_T\mid\mathcal F_s].
$$

The positive factor $D_s$ is measurable with respect to the current [filtration](../../../../../../filtration-probability-theory.md). Dividing it out gives

$$
\boxed{P_{s,T}=\mathbb E\left[\exp\left(-\int_s^TR_u\,du\right)\middle|\mathcal F_s\right].}
$$

Conversely, this identity says $Z_{s,T}=\mathbb E[D_T\mid\mathcal F_s]$. The [tower property](../../../../../../law-of-total-expectation.md) gives $\mathbb E[Z_{s,T}\mid\mathcal F_r]=Z_{r,T}$ for every $r\leq s$, establishing the [martingale](../../../../../../martingale-split.md) condition. The integrated [short rate](../../../../../../short-rate.md) is a [Gaussian random variable](../../../../../../gaussian-random-variable.md) with finite [variance](../../../../../../variance-split.md), so the [Gaussian moment-generating function](../../../../../../moment-generating-function-of-a-normal-distribution.md) proves that $D_T$ is [integrable](../../../../../../integrability.md). Together with the preceding subparts, this proves all three descriptions equivalent.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

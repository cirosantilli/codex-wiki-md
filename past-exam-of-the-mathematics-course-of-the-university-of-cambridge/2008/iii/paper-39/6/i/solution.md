<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $Q$ denote the given unique [equivalent martingale measure](../../../../../../risk-neutral-measure.md). A [zero-coupon bond](../../../../../../zero-coupon-bond.md) paying one at $T$ has [risk-neutral pricing](../../../../../../risk-neutral-pricing.md) value

$$
P_t(T)=\mathbb E_Q\left[\exp\left(-\int_t^Tr_sds\right)\middle|\mathcal F_t\right].
$$

Write $h=T-t$. Split the integrated [short rate](../../../../../../short-rate.md) into its known and future parts:

$$
\int_t^Tr_sds=\int_t^Tg(s)ds+\sigma h\widehat W_t+\sigma\int_t^T(\widehat W_s-\widehat W_t)ds.
$$

By integrating the future [Brownian motion](../../../../../../brownian-motion-split.md) increments in the opposite order, the last integral equals $\int_t^T(T-u)d\widehat W_u$. It is independent of $\mathcal F_t$ and is a [Gaussian random variable](../../../../../../gaussian-random-variable.md) of mean zero and [variance](../../../../../../variance-split.md)

$$
\int_t^T(T-u)^2du=\frac{h^3}{3}.
$$

The [Gaussian](../../../../../../normal-distribution.md) [exponential moment](../../../../../../exponential-moment.md) formula $\mathbb E[e^{aZ}]=e^{a^2\operatorname{Var}(Z)/2}$ for centered $Z$ therefore gives the bond price in this [Gaussian short-rate model with a deterministic shift](../../../../../../gaussian-short-rate-model-with-a-deterministic-shift.md):

$$
\boxed{P_t(T)=\exp\left[-\int_t^Tg(s)ds-\sigma(T-t)\widehat W_t+\frac{\sigma^2(T-t)^3}{6}\right].}
$$

The [instantaneous forward rate](../../../../../../instantaneous-forward-rate.md) is the negative maturity [derivative](../../../../../../derivative.md) of the logarithm of the bond price. Consequently

$$
\boxed{f_t(T)=g(T)+\sigma\widehat W_t-\frac{\sigma^2}{2}(T-t)^2.}
$$

In particular, $P_t(t)=1$ and $f_t(t)=g(t)+\sigma\widehat W_t=r_t$, as required. The [derivative](../../../../../../derivative.md) formula is pointwise for continuous $g$ and almost everywhere for locally integrable $g$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6](../../6.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

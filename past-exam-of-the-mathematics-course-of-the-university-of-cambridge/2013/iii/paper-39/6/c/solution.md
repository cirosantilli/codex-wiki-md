<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Here the [bank account](../../../../../../bank-account.md) is continuous and of finite variation, but for $t>0$ its rate is $r_t=t^{-1/2}$. This is integrable at zero, so the account itself is well defined. The stock satisfies $dS_t=S_tdW_t$. The previous continuity hypothesis on the rate no longer holds at the initial time.

Suppose a positive normalized [state-price density](../../../../../../state-price-density.md) existed; even a [local martingale deflator](../../../../../../local-martingale-deflator.md) would suffice for a contradiction. Then $ZB$ would be a continuous [local martingale](../../../../../../local-martingale.md) by the [Brownian martingale representation theorem](../../../../../../brownian-martingale-representation-theorem.md). Dividing by the positive continuous account gives continuous $Z$, with $Z_0=1$, and

$$
dZ_t=-Z_tt^{-1/2}dt+\eta_tdW_t,
\qquad \int_0^t\eta_s^2ds<\infty\quad\text{locally}.
$$

The [Itô product rule](../../../../../../ito-product-rule.md) for $ZS$ forces its drift to vanish, so $\eta_t=Z_tt^{-1/2}$ for almost every positive time. Continuity and $Z_0=1$ imply that each path has a positive interval on which $Z_t\ge1/2$. But then

$$
\int_0^\delta\eta_t^2dt=\int_0^\delta\frac{Z_t^2}{t}dt\ge\frac14\int_0^\delta\frac{dt}{t}=\infty,
$$

contradicting the local square-integrability required for the [stochastic integral](../../../../../../stochastic-integral.md). Thus

$$
\boxed{\text{there is no positive normalized local deflator, hence no state-price density.}}
$$

This is the [singular initial market-price-of-risk obstruction](../../../../../../singular-initial-market-price-of-risk-obstruction.md): the necessary market price of risk is $-t^{-1/2}$, whose squared integral diverges at zero. On an interval starting at a strictly positive time this particular obstruction disappears; the initial-time normalization is essential.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

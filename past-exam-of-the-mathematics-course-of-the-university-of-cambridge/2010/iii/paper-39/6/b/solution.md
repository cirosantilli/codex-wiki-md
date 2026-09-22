<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $h=S_0-\mu/R$. The initial capital of the [one-period quadratic hedge](../../../../../../one-period-quadratic-hedge.md) is

$$
X_0^*=\phi^*+(\pi^*)^TS_0
=\frac{m}{R}+h^TV^{-1}c.
$$

Define the [minimum-norm one-period pricing weight](../../../../../../minimum-norm-one-period-pricing-weight.md)

$$
\boxed{\rho^*=\frac1R+h^TV^{-1}(S_1-\mu).}
$$

It is square integrable, and $\mathbb E[(S_1-\mu)\xi_1]=c$, so

$$
\mathbb E[\rho^*\xi_1]=\frac{m}{R}+h^TV^{-1}c=X_0^*.
$$

The weight depends only on the asset prices and their first two moments, not on the claim. It can be negative, so this identity alone does not supply an [equivalent martingale measure](../../../../../../risk-neutral-measure.md) or a positive [state-price density](../../../../../../state-price-density.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

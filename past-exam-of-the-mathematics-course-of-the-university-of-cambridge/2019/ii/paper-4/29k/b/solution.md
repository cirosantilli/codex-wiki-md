<h1 id="29k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The arbitrage-free value of the discounted claim is the [conditional expectation](../../../../../../conditional-expectation.md)

$$
V_t=\mathbb E_Q[H\mid\mathcal F_t].
$$

Conditional on the observed path $(S_0^1,\ldots,S_t^1)=(x_0,\ldots,x_t)$, the future multiplicative increments are independent of $\mathcal F_t$ and have the same law as a fresh stock path divided by its initial value. Therefore

$$
\boxed{V_t(\omega)=v_t(S_0^1,S_1^1(\omega),\ldots,S_t^1(\omega)),}
$$

where

$$
\boxed{
v_t(x_0,\ldots,x_t)=
\mathbb E_Q\left[h\left(x_0,\ldots,x_t,
x_t\frac{S_1^1}{S_0^1},\ldots,
x_t\frac{S_{T-t}^1}{S_0^1}\right)\right].}
$$

This is [Risk-neutral valuation in the Cox--Ross--Rubinstein model](../../../../../../risk-neutral-valuation-in-the-cox-ross-rubinstein-model.md) for a path-dependent claim.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [29K](../../29k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

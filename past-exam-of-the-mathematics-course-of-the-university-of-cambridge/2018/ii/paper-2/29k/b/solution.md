<h1 id="29k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\tau=T-t$. Conditional on $\mathcal F_t$ under the risk-neutral measure,

$$
S_T=S_t\exp\left(\sigma(W_T^Q-W_t^Q)
+\left(r-\frac12\sigma^2\right)\tau\right).
$$

Using the [moment-generating function of a normal distribution](../../../../../../moment-generating-function-of-a-normal-distribution.md) in the risk-neutral expectation gives the [Power payoff in the Black-Scholes model](../../../../../../power-payoff-in-the-black-scholes-model.md) value

$$
\boxed{
V_t=S_t^\gamma
\exp\left[
\left((\gamma-1)r+\frac12\gamma(\gamma-1)\sigma^2\right)(T-t)
\right].}
$$

In particular,

$$
\boxed{
V_0=S_0^\gamma
\exp\left[
\left((\gamma-1)r+\frac12\gamma(\gamma-1)\sigma^2\right)T
\right].}
$$

The [delta hedge](../../../../../../delta-hedge.md) holds

$$
\boxed{
\Delta_t=\frac{\partial V}{\partial S}(t,S_t)
=\gamma S_t^{\gamma-1}
\exp\left[
\left((\gamma-1)r+\frac12\gamma(\gamma-1)\sigma^2\right)(T-t)
\right]}
$$

units of the risky asset.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [29K](../../29k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

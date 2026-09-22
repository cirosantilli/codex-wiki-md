<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set

$$
\lambda=\frac{\mu-r}{\sigma},
\qquad
\frac{dQ}{dP}
=\exp\left(-\lambda W_T-\frac12\lambda^2T\right).
$$

By the [Girsanov theorem](../../../../../../girsanov-theorem.md), $W_t^Q=W_t+\lambda t$ is Brownian motion under $Q$. Consequently

$$
dS_t=rS_t\,dt+\sigma S_t\,dW_t^Q,
$$

so discounted stock price is a martingale and $Q$ is the [Risk-neutral measure for the Black-Scholes model](../../../../../../risk-neutral-measure-for-the-black-scholes-model.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

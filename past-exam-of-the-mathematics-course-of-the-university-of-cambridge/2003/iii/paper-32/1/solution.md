<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [positive state-price density alternative](../../../../../positive-state-price-density-alternative.md) characterizes one-period [arbitrage](../../../../../arbitrage.md). Interpret $A_0$ as the vector of current asset prices and $A_1$ as their terminal payments. A fixed vector of holdings produces initial cost $x^\top A_0$ and terminal payment $x^\top A_1$. The first alternative is a nonpositive-cost investment with a nonnegative payment and strict improvement either initially or on an event of positive probability. A strictly positive [state-price density](../../../../../state-price-density.md) prices every such payment and excludes both forms of [arbitrage](../../../../../arbitrage.md), as proved below.

If there is a traded [bank account](../../../../../bank-account.md) costing one and paying a deterministic $R>0$, the density satisfies $1=R\mathbb E\nu$. Hence $dQ/dP=R\nu$ defines an [equivalent martingale measure](../../../../../risk-neutral-measure.md) and

$$
\boxed{A_0=\frac1R\mathbb E_Q A_1.}
$$

Conversely this pricing relation under an [equivalent martingale measure](../../../../../risk-neutral-measure.md) gives $\nu=R^{-1}dQ/dP$. Without such an account, $\nu$ is a pricing density, not necessarily a probability density or even an [integrable random variable](../../../../../integrable-random-variable.md) by itself; the stated requirement is [integrability](../../../../../integrability.md) of $\nu A_1$. This distinction keeps the abstract alternative valid without an unstated asset paying one.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

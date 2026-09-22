<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Suppose $Q$ is an [equivalent martingale measure](../../../../../../risk-neutral-measure.md) and a zero-cost [self-financing strategy](../../../../../../self-financing-portfolio.md) has holdings $(h_B,h_S)$. Its discounted terminal value has [conditional expectation](../../../../../../conditional-expectation.md)

$$
\mathbb E_Q[V_1/B_1\mid\mathcal F_0]=h_B+h_S\mathbb E_Q[S_1/B_1\mid\mathcal F_0]=h_B+h_SS_0/B_0=V_0/B_0=0.
$$

If it were an [arbitrage](../../../../../../arbitrage.md), $V_1/B_1$ would be nonnegative because $B_1>0$. Equivalence implies that it is strictly positive on an event of positive $Q$-probability. A nonnegative [random variable](../../../../../../random-variable-split.md) with zero [conditional expectation](../../../../../../conditional-expectation.md) must be zero almost surely, a contradiction. Thus $\boxed{\text{an equivalent martingale measure excludes arbitrage}}$. The calculation uses the usual integrable one-period strategies, and also works conditionally for finite initial-information-measurable holdings.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

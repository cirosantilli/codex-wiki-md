<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [martingale deflator](../../../../../../martingale-deflator.md) is a strictly positive adapted process $Y$ such that every deflated cum-dividend asset gain has zero conditional drift:

$$
\mathbb E\!\left[Y_t(P_t+\delta_t)\mid\mathcal F_{t-1}\right]
=Y_{t-1}P_{t-1}.
$$

Using the definitions of $\pi^H$ and $\xi^H$,

$$
Z_t-Z_{t-1}
=H_t\mathbin\cdot
\left[Y_t(P_t+\delta_t)-Y_{t-1}P_{t-1}\right].
$$

The holdings $H_t$ are $\mathcal F_{t-1}$-measurable, so the right side is a [martingale transform](../../../../../../martingale-transform.md) of the deflated asset-gain local martingale. Hence $Z$ is a [local martingale](../../../../../../local-martingale.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

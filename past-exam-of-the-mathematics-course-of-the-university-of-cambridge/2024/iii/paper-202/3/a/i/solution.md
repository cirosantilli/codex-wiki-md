<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Fix $0\leq r\leq t$. Since $M$ is a [martingale](../../../../../../../martingale-split.md),

$$
\operatorname{Cov}(M_{t+s}-M_t,M_r)=\mathbb E\!\left[M_r\,\mathbb E[M_{t+s}-M_t\mid\mathcal F_t]\right]=0.
$$

Every finite vector consisting of $M_{t+s}-M_t$ and past values $M_{r_1},\ldots,M_{r_n}$ has a [multivariate normal distribution](../../../../../../../multivariate-normal-distribution.md). Therefore [uncorrelated jointly normal variables are independent](../../../../../../../uncorrelated-jointly-normal-variables-are-independent.md), so the increment is independent of every finite vector of past values. A [Monotone class theorem](../../../../../../../monotone-class-theorem.md) then extends this to independence from $\mathcal F_t=\sigma(M_r:0\leq r\leq t)$. This is the [independent increments of a Gaussian martingale](../../../../../../../independent-increments-of-a-gaussian-martingale.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 202](../../../../paper-202-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

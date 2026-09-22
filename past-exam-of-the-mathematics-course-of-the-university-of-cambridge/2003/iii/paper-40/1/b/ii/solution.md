<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For individual $i$, let $X_i=\min(T_i,c_i)$ and $\Delta_i=\mathbf1_{\{T_i\le c_i\}}$. The preceding [expectation](../../../../../../../expected-value.md) calculation applies separately at each fixed [censoring](../../../../../../../censoring-statistics.md) time:

$$
E[H(X_i)]=\theta E[X_i]=1-e^{-\theta c_i}=E[\Delta_i].
$$

Summing and using linearity of [expectation](../../../../../../../expected-value.md), with $D=\sum_i\Delta_i$ the failure count, gives

$$
\boxed{\sum_{i=1}^nE[H(X_i)]=\theta\sum_{i=1}^nE[X_i]=E[D].}
$$

This identity needs the stated marginal [exponential distributions](../../../../../../../exponential-distribution.md), but not independence between individuals; independence will be needed for the product [likelihood](../../../../../../../likelihood-function.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

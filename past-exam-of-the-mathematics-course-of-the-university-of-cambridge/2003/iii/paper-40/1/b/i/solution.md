<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $X=\min(T,c)$ and $\Delta=\mathbf1_{\{T\le c\}}$ for the [right-censored](../../../../../../../right-censoring.md) [survival time](../../../../../../../survival-time.md) and observed-failure indicator. Since the [exponential distribution](../../../../../../../exponential-distribution.md) is continuous, including or excluding equality at $c$ makes no difference. Using the tail-integral expression for an [expectation](../../../../../../../expected-value.md),

$$
E[X]=\int_0^cP(T>u)\,du=\int_0^c e^{-\theta u}\,du=\frac{1-e^{-\theta c}}{\theta}.
$$

Consequently the expected [integrated hazard](../../../../../../../cumulative-hazard-function.md) at the observed endpoint satisfies

$$
\boxed{E[H(X)]=\theta E[X]=1-e^{-\theta c}=P(T\le c)=E[\Delta].}
$$

[Administrative censoring](../../../../../../../administrative-censoring.md) therefore stops both the accumulated exposure and the opportunity to record a failure.

## ↑ Ancestors (12)

1. [I](../i.md)
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

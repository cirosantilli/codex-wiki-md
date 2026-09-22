<h1 id="2/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For $X_i=k/U_i$, the indicator is always one, and the [importance weight](../../../../../../../importance-weight.md) reduces to

$$
\frac{f(X_i)}{g(X_i)}=\frac{X_i^2}{\pi k(1+X_i^2)}=\frac{k}{\pi(U_i^2+k^2)}.
$$

Averaging these independent contributions gives

$$
\boxed{\widehat\mu=\frac1n\sum_{i=1}^n\frac{k}{\pi(U_i^2+k^2)}.}
$$

As a direct normalization check, its [expectation](../../../../../../../expected-value.md) is $\int_0^1 k/[\pi(u^2+k^2)]\,du=\pi^{-1}\arctan(1/k)$. For $k>0$ this equals $1/2-\pi^{-1}\arctan k$, the exact standard [Cauchy distribution](../../../../../../../cauchy-distribution.md) tail [probability](../../../../../../../probability.md). The substitution $X=k/U$, rather than $k/(1-U)$ with the same symbol left unchanged, explains why the displayed denominator contains $U^2$.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2002](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

By the [Itô formula](../../../../../../ito-s-lemma.md),

$$
f(X_t)-f(X_0)=\int_0^tf'(X_s)\,dX_s+\frac12\int_0^tf''(X_s)\,d[X]_s.
$$

To compute the [Stratonovich integral](../../../../../../stratonovich-integral.md) correction, apply the [Itô formula](../../../../../../ito-s-lemma.md) also to $f'$, which is twice continuously differentiable because $f$ is $C^3$. The continuous [local martingale](../../../../../../local-martingale.md) part of $f'(X)$ is $\int f''(X_s)dL_s$, where $L$ is the continuous [local martingale](../../../../../../local-martingale.md) part of $X$. A [finite-variation process](../../../../../../finite-variation-process.md) has zero [quadratic covariation](../../../../../../quadratic-covariation.md) with $X$, and the [quadratic variation of a stochastic integral](../../../../../../quadratic-variation-of-a-stochastic-integral.md) together with [polarization identity](../../../../../../polarization-identity.md) gives

$$
[f'(X),X]_t=\int_0^tf''(X_s)\,d[X]_s.
$$

All these statements can be localized to compact ranges of $X$, so unbounded derivatives create no global integrability requirement. Substitute this identity into the [Stratonovich integral](../../../../../../stratonovich-integral.md) to obtain the [Stratonovich chain rule](../../../../../../stratonovich-chain-rule.md):

$$
\boxed{f(X_t)-f(X_0)=\int_0^tf'(X_s)\,\partial X_s.}
$$

This is the integrated meaning of the requested differential identity; there is no extra second-order term after the [Stratonovich integral](../../../../../../stratonovich-integral.md) correction has been included.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

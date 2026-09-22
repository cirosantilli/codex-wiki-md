<h1 id="13k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $Y_i=X_i^T\beta+\varepsilon_i$, where conditionally $\mathbb E(\varepsilon_i|X_i)=0$ and $\operatorname{Var}(\varepsilon_i|X_i)=\sigma^2v(X_i)$. Then

$$
\widehat\beta(\Sigma)-\beta=
\left(\frac1n\sum_i\frac{X_iX_i^T}{v(X_i)}\right)^{-1}
\frac1n\sum_i\frac{X_i\varepsilon_i}{v(X_i)}.
$$

The law of large numbers sends the [matrix](../../../../../../matrix.md) to

$$
A=\mathbb E\left[\frac{XX^T}{v(X)}\right],
$$

while the [vector](../../../../../../vector.md) tends to zero, proving consistency. The central [limit](../../../../../../limit-of-a-function.md) theorem and Slutsky's theorem give

$$
\sqrt n(\widehat\beta(\Sigma)-\beta)\Rightarrow N(0,\sigma^2A^{-1}).
$$

Similarly, with $B=\mathbb E(XX^T)$ and $C=\mathbb E(v(X)XX^T)$,

$$
\sqrt n(\widehat\beta(I)-\beta)\Rightarrow
N(0,\sigma^2B^{-1}CB^{-1}).
$$

These conclusions require the displayed [matrices](../../../../../../matrix.md) to be finite and nonsingular.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [13K](../../13k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

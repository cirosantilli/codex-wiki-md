<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [code-distribution correspondence](../../../../../../code-distribution-correspondence.md) starts from the [Kraft inequality](../../../../../../kraft-mcmillan-inequality.md). For codeword lengths $L(x)$ put

$$
K=\sum_x2^{-L(x)}\leq1,
\qquad
R(x)=\frac{2^{-L(x)}}K.
$$

Conversely, a probability mass function determines ideal lengths $-\log_2R(x)$, up to integer rounding. For the source law $P_n$,

$$
\begin{aligned}
\mathbb E L(X_1^n)
&=-\sum_xP_n(x)\log_2\{K R(x)\}\\
&=H(P_n)+D(P_n\|R)-\log_2K\\
&\geq H(X_1^n),
\end{aligned}
$$

using nonnegativity of [Kullback-Leibler divergence](../../../../../../kullback-leibler-divergence.md) and $K\leq1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

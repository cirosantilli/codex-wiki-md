<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $K>0$, the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and part a give

$$
\mathbb E\left[Y_n^-\mathbf1_{\{Y_n^->K\}}\right]
\leq\sqrt{\mathbb E[(Y_n^-)^2]}
\sqrt{\mathbb P(Y_n^->K)}
\leq\frac1K.
$$

Thus $(Y_n^-)$ is [uniformly integrable](../../../../../../uniform-integrability.md). Combining this with the [weak convergence of random variables](../../../../../../convergence-in-distribution.md) from part b yields convergence of the first moments:

$$
\mathbb E[Y_n^-]\longrightarrow\mathbb E[Y^-].
$$

By symmetry of the standard normal density,

$$
\mathbb E[Y^-]
=\int_0^\infty x\frac{e^{-x^2/2}}{\sqrt{2\pi}}\,dx
=\frac1{\sqrt{2\pi}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

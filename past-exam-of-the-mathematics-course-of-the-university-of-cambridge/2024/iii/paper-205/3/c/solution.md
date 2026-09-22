<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For each column $X_j$, the normalized score is

$$
W_j=\frac1nX_j^T\varepsilon=\frac1n\sum_{i=1}^nX_{ij}\varepsilon_i.
$$

The errors are independent [Rademacher random variables](../../../../../../rademacher-distribution.md), and $\lVert X_j\rVert_2^2=n$. The [Hoeffding lemma](../../../../../../hoeffding-lemma.md) therefore makes $W_j$ a [sub-Gaussian random variable](../../../../../../sub-gaussian-distribution.md) with variance proxy $1/n$, so

$$
\mathbb P(|W_j|>t)\leq2e^{-nt^2/2}.
$$

The [union bound](../../../../../../boole-s-inequality.md) with $t=\lambda/2$ gives

$$
\mathbb P(\Omega)
\geq1-2p\exp\!\left(-\frac{n\lambda^2}{8}\right).
$$

For $\lambda=A\sqrt{\log p/n}$ this becomes

$$
\mathbb P(\Omega)\geq1-2p^{,1-A^2/8}.
$$

In particular, if $A>\sqrt8$, the lower bound tends to one as $p\to\infty$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

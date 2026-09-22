<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\delta=\widehat\beta-\beta^0$. Standard [sub-Gaussian random variable](../../../../../../sub-gaussian-distribution.md) and Gaussian-product concentration gives, for $n>\log p$,

$$
\mathbb P\left(\left\lVert\frac1nX^T\varepsilon\right\rVert_\infty
>A\sigma v\sqrt{\frac{\log p}{n}}\right)
\leq2p\exp(-A^2\log p/8).
$$

Thus $A=4$ makes this probability at most $2/p$. On the complementary event, the basic inequality and [Holder inequality](../../../../../../holder-inequality.md) give

$$
\frac1n\lVert X\delta\rVert_2^2
\leq\lambda\bigl(\lVert\delta\rVert_1+
\lVert\beta^0\rVert_1-\lVert\widehat\beta\rVert_1\bigr).
$$

The parenthesis is at most $2\lVert\delta\rVert_1$ by the triangle inequality and at most $2\lVert\beta^0\rVert_1$ by $\lVert\delta\rVert_1\leq\lVert\widehat\beta\rVert_1+\lVert\beta^0\rVert_1$. Substituting $\lambda=A\sigma v\sqrt{\log p/n}$ proves $\Omega_1$, whose probability tends to one.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\widehat\Sigma=X^TX/n$. Direct substitution of $Y=X\beta^0+\varepsilon$ into the [Debiased Lasso](../../../../../../debiased-lasso.md) gives

$$
\sqrt n(\widehat b-\beta^0)
=\underbrace{\frac1{\sqrt n}\widehat\Theta^TX^T\varepsilon}_{W}
+\underbrace{\sqrt n(I-\widehat\Theta^T\widehat\Sigma)(\widehat\beta-\beta^0)}_{\Delta}.
$$

Conditionally on the deterministic design,

$$
\boxed{W\sim N_p(0,\widehat\Theta^T\widehat\Sigma\widehat\Theta)}.
$$

The assumed [approximate inverse of a Gram matrix](../../../../../../approximate-inverse-of-a-gram-matrix.md) property and [Holder inequality](../../../../../../holder-inequality.md) imply

$$
\lVert\Delta\rVert_\infty
\leq\sqrt n\lVert I-\widehat\Theta^T\widehat\Sigma\rVert_{\max}
\lVert\widehat\beta-\beta^0\rVert_1
\leq\sqrt{\log p}\,\lVert\widehat\beta-\beta^0\rVert_1.
$$

**Thus $\rho(n,p)=\sqrt{\log p}$.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

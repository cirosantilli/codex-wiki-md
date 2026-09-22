<h1 id="29k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For observations $X_1,\ldots,X_n$, the [log-likelihood](../../../../../../log-likelihood.md) is, up to an additive constant,

$$
\ell(\sigma)=-n\log\sigma-\frac1{2\sigma^2}\sum_iX_i^2.
$$

Its unique maximum is

$$
\widehat\sigma_{\rm MLE}=\sqrt{\frac1n\sum_iX_i^2}.
$$

Now $\mathbb E[X_i^2]=\sigma^2$ and, using $\mathbb E[Z^4]=3$, $\operatorname{Var}(X_i^2)=2\sigma^4$. The [central limit theorem](../../../../../../central-limit-theorem.md) followed by the [delta method](../../../../../../delta-method.md) for $g(x)=\sqrt x$ gives

$$
\boxed{\sqrt n(\widehat\sigma_{\rm MLE}-\sigma)
\xrightarrow dN(0,\sigma^2/2)}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [29K](../../29k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

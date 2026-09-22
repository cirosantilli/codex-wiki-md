<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [regression residual](../../../../../../regression-residual.md) vector is $e=Y-X\widehat\beta=(I-H)Y$, where $H=X(X^TX)^{-1}X^T$ is the [hat matrix](../../../../../../hat-matrix.md). Both $H$ and $I-H$ are symmetric [idempotent](../../../../../../idempotent.md) matrices, and $(I-H)X=0$. Therefore $e=(I-H)\varepsilon$ and the [linear image of a multivariate normal vector](../../../../../../linear-image-of-a-multivariate-normal-vector.md) gives

$$
\boxed{e\sim N_n\bigl(0,\sigma^2(I-H)\bigr).}
$$

This [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) is singular, with rank $n-p$: [fitted-residual orthogonality](../../../../../../fitted-residual-orthogonality.md) forces $X^Te=0$. Specifically, $\operatorname{Var}(e_i)=\sigma^2(1-h_{ii})$ and $\operatorname{Cov}(e_i,e_j)=-\sigma^2h_{ij}$ for distinct observations. Thus [regression residuals](../../../../../../regression-residual.md) are generally neither independent nor identically distributed, even though the model errors are. Also $\operatorname{RSS}/\sigma^2\sim\chi^2_{n-p}$ and is independent of $\widehat\beta$, which justifies the [standard errors](../../../../../../standard-error.md) and exact [Student t-tests](../../../../../../student-s-t-test.md) below.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

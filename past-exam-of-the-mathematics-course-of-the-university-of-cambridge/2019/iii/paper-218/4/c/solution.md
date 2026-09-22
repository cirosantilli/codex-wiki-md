<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

When $p>n$, the pooled within-class covariance has rank at most $n-L<p$, so it is singular and ordinary LDA is not defined. For every $\lambda>0$,

$$
\widehat\Sigma_\lambda=\widehat\Sigma+\lambda I
$$

is positive definite because $v^T\widehat\Sigma_\lambda v\geq\lambda\|v\|^2>0$. Replacing the covariance by this matrix gives well-defined regularized LDA. Choose $\lambda$ for predictive performance by [cross-validation](../../../../../../cross-validation.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="o/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Differentiating the least-squares residual norm gives the [normal equations](../../../../normal-equation.md)

$$
X^TX\hat\theta=X^TY.
$$

If $X$ has full column rank, $\hat\theta=(X^TX)^{-1}X^TY$, and therefore

$$
\operatorname{Var}(\hat\theta)
=(X^TX)^{-1}X^T(\sigma^2I)X(X^TX)^{-1}
=\sigma^2(X^TX)^{-1}.
$$

Here $\bar x=0$ and $\bar z=2$, so the [design matrix](../../../../design-matrix.md) and its Gram matrix are

$$
X=\begin{pmatrix}
1&-3&1\\1&-2&0\\1&-1&-1\\
1&1&-1\\1&2&0\\1&3&1
\end{pmatrix},\qquad
X^TX=\operatorname{diag}(6,28,4).
$$

The centered predictor columns are perpendicular, giving

$$
\boxed{\operatorname{Cov}(\hat\beta,\hat\gamma)=0,\qquad
\operatorname{Var}(\hat\beta)=\sigma^2/28,\quad
\operatorname{Var}(\hat\gamma)=\sigma^2/4.}
$$

Both estimates are linear combinations of the jointly normal errors, hence jointly normal. Zero covariance therefore also gives **independence**. The normality assumption is what permits this last step; orthogonality alone would only prove uncorrelatedness.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [O](../../o.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

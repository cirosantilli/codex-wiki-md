<h1 id="o/o2/solution">Solution</h1>

↑ **Parent:** [O2](../o2.md)

The [normal equations for linear least squares](../../../../normal-equations-for-linear-least-squares.md) are $X^TX\widehat\theta=X^TY$. Under full column rank, $\widehat\theta=(X^TX)^{-1}X^TY$. Since $\operatorname{Cov}(Y)=\sigma^2I$,

$$
\boxed{\operatorname{Cov}(\widehat\theta)=\sigma^2(X^TX)^{-1}X^TX(X^TX)^{-1}=\sigma^2(X^TX)^{-1}}.
$$

Here $\bar x=0$ and $\bar z=2$, so the design matrix is

$$
\boxed{X=\begin{pmatrix}1&-3&1\\1&-2&0\\1&-1&-1\\1&1&-1\\1&2&0\\1&3&1\end{pmatrix}}.
$$

Its columns are pairwise orthogonal and have squared lengths $6,28,4$. Consequently $X^TX=\operatorname{diag}(6,28,4)$, giving

$$
\boxed{\operatorname{Var}(\widehat\beta)=\frac{\sigma^2}{28},\quad\operatorname{Var}(\widehat\gamma)=\frac{\sigma^2}4,\quad\operatorname{Cov}(\widehat\beta,\widehat\gamma)=0}.
$$

Both estimators are linear functions of the [Jointly Gaussian](../../../../multivariate-normal-distribution.md) observation vector, so they are [Jointly Gaussian](../../../../multivariate-normal-distribution.md). Zero covariance then implies **[independence](../../../../independent-random-variables.md)**. This final implication uses the normal error model, whereas the [variance](../../../../variance-split.md) calculation itself needs only its second moments.

## ↑ Ancestors (12)

1. [O2](../o2.md)
2. [O](../../o.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

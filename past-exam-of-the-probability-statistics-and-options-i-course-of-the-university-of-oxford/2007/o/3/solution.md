<h1 id="o/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Minimizing the squared residual norm gives the [normal equations](../../../../normal-equation.md)

$$
\boxed{X^TX\,\widehat\theta=X^TY.}
$$

Full column rank makes $X^TX$ invertible. With columns corresponding to $1,x,x^2-4$, the [design matrix](../../../../design-matrix.md) is

$$
X=\begin{pmatrix}
1&-3&5\\1&-2&0\\1&-1&-3\\1&0&-4\\
1&1&-3\\1&2&0\\1&3&5
\end{pmatrix}.
$$

Symmetry gives zero cross products between the odd column and either even column, and $\sum(x^2-4)=28-28=0$ gives the remaining orthogonality. Their squared norms are seven, 28 and 84, so $X^TX=\operatorname{diag}(7,28,84)$. Therefore

$$
\boxed{\widehat\alpha=\frac17\sum_{j=1}^7y_j,}
$$



$$
\boxed{\widehat\beta=
\frac{-3y_1-2y_2-y_3+y_5+2y_6+3y_7}{28},}
$$



$$
\boxed{\widehat\gamma=
\frac{5y_1-3y_3-4y_4-3y_5+5y_7}{84}.}
$$

Since the error [covariance](../../../../covariance.md) is $\sigma^2I$, [least squares](../../../../least-squares.md) has [covariance](../../../../covariance.md) $\sigma^2(X^TX)^{-1}$. Thus

$$
\boxed{\operatorname{Var}\widehat\alpha=\frac{\sigma^2}7,\quad
\operatorname{Var}\widehat\beta=\frac{\sigma^2}{28},\quad
\operatorname{Var}\widehat\gamma=\frac{\sigma^2}{84}.}
$$

The estimators have zero [covariances](../../../../covariance.md). [independence](../../../../independent-random-variables.md) would require an additional distributional assumption such as Gaussian errors; the stated mean and [variance](../../../../variance-split.md) assumptions alone give only the [covariance](../../../../covariance.md) calculation.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [O](../../o.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

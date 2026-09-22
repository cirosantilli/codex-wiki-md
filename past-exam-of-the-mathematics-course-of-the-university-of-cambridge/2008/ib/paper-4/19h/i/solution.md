<h1 id="19h/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume the explanatory variables are not all equal, so $S_{xx}=\sum_i(x_i-\bar x)^2>0$. In the [Gaussian linear model](../../../../../../normal-linear-model.md), the [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell(\alpha,\beta,\sigma^2)=-\frac n2\log(2\pi\sigma^2)-\frac1{2\sigma^2}\sum_{i=1}^n(Y_i-\alpha-\beta x_i)^2.
$$

For fixed $\sigma^2$, [maximum likelihood estimation](../../../../../../maximum-likelihood-estimation.md) therefore minimizes the [residual sum of squares](../../../../../../residual-sum-of-squares.md). Differentiating in $\alpha,\beta$ gives the [least-squares normal equations](../../../../../../normal-equations-for-linear-least-squares.md)

$$
\sum_i(Y_i-\widehat\alpha-\widehat\beta x_i)=0,\qquad\sum_ix_i(Y_i-\widehat\alpha-\widehat\beta x_i)=0.
$$

The first gives $\widehat\alpha=\bar Y-\widehat\beta\bar x$; substituting it into the second gives $\widehat\beta=S_{xy}/S_{xx}$, with $S_{xy}=\sum_i(x_i-\bar x)(Y_i-\bar Y)$. Let $\operatorname{SSE}=\sum_i(Y_i-\widehat\alpha-\widehat\beta x_i)^2$. Differentiating the profiled [log-likelihood](../../../../../../log-likelihood.md) in $\sigma^2$ gives

$$
\boxed{\widehat\beta=\frac{S_{xy}}{S_{xx}},\qquad\widehat\alpha=\bar Y-\widehat\beta\bar x,\qquad\widehat{\sigma^2}=\frac{\operatorname{SSE}}n.}
$$

For the variance estimator this is the interior maximum when $\operatorname{SSE}>0$, which occurs almost surely under the model when $n>2$.

The coefficient estimators are linear functions of the independent normal errors. In particular,

$$
\widehat\beta-\beta=\frac{\sum_i(x_i-\bar x)\varepsilon_i}{S_{xx}},\qquad\widehat\alpha-\alpha=\bar\varepsilon-\bar x(\widehat\beta-\beta).
$$

Their [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) has mean $(\alpha,\beta)^T$ and [covariance matrix](../../../../../../covariance-matrix.md)

$$
\sigma^2\begin{pmatrix}1/n+\bar x^2/S_{xx}&-\bar x/S_{xx}\\-\bar x/S_{xx}&1/S_{xx}\end{pmatrix}.
$$

The fitted vector is the [orthogonal projection](../../../../../../orthogonal-projection.md) onto the two-dimensional span of $(1,\ldots,1)^T$ and $(x_1,\ldots,x_n)^T$. The residual vector is the complementary projection of the spherical normal error vector. Orthogonal normal projections are independent, and in an [orthonormal basis](../../../../../../orthonormal-basis.md) of that complementary space its $n-2$ coordinates are independent $N(0,\sigma^2)$. Consequently

$$
\frac{\operatorname{SSE}}{\sigma^2}=\frac{n\widehat{\sigma^2}}{\sigma^2}\sim\chi^2_{n-2},
$$

independently of $(\widehat\alpha,\widehat\beta)$. This also gives the [unbiased estimator](../../../../../../unbiased-estimator.md) $s^2=\operatorname{SSE}/(n-2)$ rather than the variance MLE.

Under the [null hypothesis](../../../../../../null-hypothesis.md) $\alpha=0$, for $n>2$ the [Student t test for a simple-regression intercept](../../../../../../student-t-test-for-a-simple-regression-intercept.md) uses

$$
\boxed{T=\frac{\widehat\alpha}{s\sqrt{1/n+\bar x^2/S_{xx}}}\sim t_{n-2},\qquad \text{reject if }|T|>t_{n-2,1-\eta/2}.}
$$

Here $\eta$ is the prescribed [significance level](../../../../../../significance-level.md). The normal numerator divided by its true standard deviation is independent of $(n-2)s^2/\sigma^2$, which proves the stated [Student t-distribution](../../../../../../student-s-t-distribution.md). If $S_{xx}=0$, the two coefficients are not separately identifiable; if $n\leq2$, this residual-variance-based test is unavailable.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [19H](../../19h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

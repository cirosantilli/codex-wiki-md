<h1 id="o/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Minimize the [residual sum of squares](../../../../residual-sum-of-squares.md) $\|Y-X\theta\|^2$. Differentiating gives the [normal equations](../../../../normal-equation.md) $X^TX\widehat\theta=X^TY$. [Full column rank](../../../../full-column-rank.md) makes $X^TX$ positive definite and invertible, so the unique minimizer is

$$
\boxed{\widehat\theta=(X^TX)^{-1}X^TY.}
$$

Since $\mathbb EY=X\theta$, it is unbiased. The independent common-variance errors give $\operatorname{Cov}(Y)=\sigma^2I$, hence

$$
\boxed{\operatorname{Cov}(\widehat\theta)=\sigma^2(X^TX)^{-1}.}
$$

Independent [Gaussian errors](../../../../gaussian-error.md) with common [variance](../../../../variance-split.md) are a sufficient condition for this [estimator](../../../../estimator.md) also to be the maximum likelihood [estimator](../../../../estimator.md): their log-likelihood differs from $-\|Y-X\theta\|^2/(2\sigma^2)$ by terms independent of $\theta$. Profiling an unknown common [variance](../../../../variance-split.md) gives the same minimizer. Mean and [variance](../../../../variance-split.md) assumptions alone do not specify a likelihood.

For the seven design points, $\bar x=0$ and $\overline{x^2}=4$. In increasing time order the [design matrix](../../../../design-matrix.md) is

$$
X=\begin{pmatrix}
1&-3&5\\1&-2&0\\1&-1&-3\\1&0&-4\\1&1&-3\\1&2&0\\1&3&5
\end{pmatrix}.
$$

Its columns are mutually [orthogonal](../../../../orthogonal-vectors.md): the odd sums vanish and $\sum(x_i^2-4)=0$. Their squared lengths are $7,28,84$, respectively. Therefore

$$
X^TX=\operatorname{diag}(7,28,84),\qquad
\boxed{\operatorname{Var}(\widehat\alpha)=\frac{\sigma^2}7,\quad
\operatorname{Var}(\widehat\beta)=\frac{\sigma^2}{28},\quad
\operatorname{Var}(\widehat\gamma)=\frac{\sigma^2}{84}.}
$$

In particular $\widehat\gamma=\sum_i(x_i^2-4)Y_i/84$. Testing for a quadratic contribution means testing $H_0:\gamma=0$ against $\gamma\ne0$.

The cooling measurements are stated to have zero-mean errors and known common [variance](../../../../variance-split.md), but normality is not explicitly assumed for them. Under the independent-error [linear regression model](../../../../linear-regression-model.md) as stated, [Chebyshev's inequality](../../../../chebyshev-s-inequality.md) gives a valid conservative level-$\delta$ test: reject when

$$
\boxed{|\widehat\gamma|\ge\frac{\sigma}{\sqrt{84\delta}}.}
$$

Its null rejection [probability](../../../../probability.md) is at most $\delta$ because the [estimator](../../../../estimator.md) has mean zero and the calculated [variance](../../../../variance-split.md). If [Gaussian errors](../../../../gaussian-error.md) are additionally assumed, the sharper exact test uses $Z=\sqrt{84}\widehat\gamma/\sigma\sim N(0,1)$ under the null and rejects for $|Z|>z_{1-\delta/2}$. With only seven observations, exact normal calibration cannot be deduced from the printed moment assumptions alone.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [O](../../o.md)
3. [2005](../../../2005-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

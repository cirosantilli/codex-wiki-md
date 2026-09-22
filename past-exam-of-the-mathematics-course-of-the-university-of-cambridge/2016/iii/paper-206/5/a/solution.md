<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

At a target $x$, approximate the unknown mean locally by $a+b(X_i-x)$ and solve the [local linear regression](../../../../../../local-linear-regression.md) weighted least-squares problem

$$
(\widehat a_x,\widehat b_x)=\arg\min_{a,b}\sum_{i=1}^n w_i(x)\{Y_i-a-b(X_i-x)\}^2,
\qquad w_i(x)=K\!\left(\frac{X_i-x}{h}\right),
$$

where $K$ is a nonnegative [regression kernel](../../../../../../kernel-for-nonparametric-regression.md) and $h>0$ a [smoothing bandwidth](../../../../../../smoothing-bandwidth.md). A common factor $1/h$ in all weights makes no difference. Estimate $f(x)$ by the fitted intercept $\widehat a_x$, and optionally $f'(x)$ by $\widehat b_x$. Repeat at each target rather than fitting a single global straight line.

For an explicit expression put $S_k=\sum_iw_i(X_i-x)^k$ and $T_k=\sum_iw_i(X_i-x)^kY_i$. The [normal equations](../../../../../../normal-equation.md) yield

$$
\boxed{\widehat f(x)=\frac{S_2T_0-S_1T_1}{S_0S_2-S_1^2}
=\sum_i\frac{w_i[S_2-S_1(X_i-x)]}{S_0S_2-S_1^2}\,Y_i.}
$$

The denominator is positive provided there are at least two distinct positively weighted predictor values. The weights sum to one and their first centered moment is zero, so [local linear regression](../../../../../../local-linear-regression.md) exactly reproduces affine functions and reduces boundary bias compared with a local constant fit. Smaller $h$ uses more local detail and increases [variance](../../../../../../variance-split.md); larger $h$ smooths more and can increase [bias](../../../../../../bias-of-an-estimator.md). Choose the bandwidth by [cross-validation](../../../../../../cross-validation.md) or another justified criterion. A nearest-neighbour span provides an adaptive bandwidth, as in the local fits used later.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

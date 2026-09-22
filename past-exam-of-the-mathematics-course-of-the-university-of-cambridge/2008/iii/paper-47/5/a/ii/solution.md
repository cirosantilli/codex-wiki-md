<h1 id="5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the shape-scale convention for the [inverse-gamma distribution](../../../../../../../inverse-gamma-distribution.md): $\operatorname{IG}(a,b)$ has density proportional to $s^{-a-1}e^{-b/s}$ for $s>0$. Write $X=X_k$, $\beta=\beta_k$, $\mu=\mu_k$, $\Sigma=\Sigma_k$ and $s=\sigma^2$. The [independent normal and inverse-gamma regression priors](../../../../../../../independent-normal-and-inverse-gamma-regression-priors.md) make the conditional [log-likelihood](../../../../../../../log-likelihood.md) plus log prior in $\beta$ equal, up to a constant, to

$$
-\frac12\left[\beta^T(X^TX/s+\Sigma^{-1})\beta
 -2\beta^T(X^Ty/s+\Sigma^{-1}\mu)\right].
$$

Define $V=(X^TX/s+\Sigma^{-1})^{-1}$ and $m=V(X^Ty/s+\Sigma^{-1}\mu)$. [Completing the square](../../../../../../../completing-the-square.md) turns this expression into $-(\beta-m)^TV^{-1}(\beta-m)/2$ plus a constant. Thus the conditional [posterior distribution](../../../../../../../bayesian-posterior.md) is the [multivariate normal distribution](../../../../../../../multivariate-normal-distribution.md)

$$
\boxed{\beta_k\mid\sigma^2,x,y\sim N_{k+1}(m,V),\quad
V=(X_k^TX_k/\sigma^2+\Sigma_k^{-1})^{-1},\quad
m=V(X_k^Ty/\sigma^2+\Sigma_k^{-1}\mu_k).}
$$

Positive definiteness of the prior [covariance matrix](../../../../../../../covariance-matrix.md) makes this well defined even if the [design matrix](../../../../../../../design-matrix.md) is rank deficient.

Holding $\beta$ fixed, the factors depending on $s$ are

$$
s^{-(a+n/2)-1}\exp\left(-\frac{b+\|y-X\beta\|^2/2}{s}\right).
$$

Consequently

$$
\boxed{\sigma^2\mid\beta_k,x,y\sim\operatorname{IG}\left(a+n/2,\ b+\tfrac12\|y-X_k\beta_k\|^2\right).}
$$

There is no additional $(k+1)/2$ in the shape: the [normal distribution](../../../../../../../normal-distribution.md) prior for $\beta_k$ is independent of $\sigma^2$. A prior scaled by $\sigma^2$ would be a different model and would change that calculation.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

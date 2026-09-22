<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Represent the subset model by a set $M$ of $k$ column indices and let $X_M$ contain those columns. Its [ordinary least squares](../../../../../ordinary-least-squares.md) estimator sets the omitted coefficients to zero and has

$$
\widehat\theta_M=(X_M^TX_M)^{-1}X_M^TY,\qquad X\widehat\theta^M=P_MY,\qquad P_M=X_M(X_M^TX_M)^{-1}X_M^T.
$$

For $k=0$, use $P_M=0$. [Full column rank](../../../../../full-column-rank.md) of $X$ implies [full column rank](../../../../../full-column-rank.md) for each $X_M$. The matrix $P_M$ is an [orthogonal projection matrix](../../../../../orthogonal-projection-matrix.md) of rank $k$.

Put $\mu=X\theta$ and $b_M=(I-P_M)\mu$. Projection [orthogonality](../../../../../orthogonal-vectors.md) gives the [bias-variance decomposition of mean squared error](../../../../../bias-variance-decomposition-of-mean-squared-error.md)

$$
R(M)=\mathbb E\|P_MY-\mu\|^2=\|b_M\|^2+k\sigma^2,
$$

while the expected [residual sum of squares](../../../../../residual-sum-of-squares.md) is

$$
\mathbb E\|(I-P_M)Y\|^2=\|b_M\|^2+(n-k)\sigma^2.
$$

These equations distinguish the [mean-vector prediction risk](../../../../../mean-vector-prediction-risk.md) in this problem from the additional noise in predicting a new response vector.

First take $p<n$. Let $P_X$ project onto the full column space of $X$. Since the full model contains $\mu$, the [residual estimate of Gaussian noise variance](../../../../../residual-estimate-of-gaussian-noise-variance.md)

$$
\widehat\sigma^2=\frac{\|(I-P_X)Y\|^2}{n-p}
$$

is unbiased: its numerator has expectation $(n-p)\sigma^2$. Consequently an [unbiased Gaussian projection risk estimate](../../../../../unbiased-gaussian-projection-risk-estimate.md) is

$$
\boxed{\widehat R(M)=\|(I-P_M)Y\|^2+(2k-n)\widehat\sigma^2.}
$$

Indeed its expectation is $\|b_M\|^2+(n-k)\sigma^2+(2k-n)\sigma^2=R(M)$ for every $\theta$, even when the subset model omits true effects. [Independence](../../../../../independent-random-variables.md) of the two terms is not needed for this expectation calculation. The full-model [variance](../../../../../variance-split.md) estimate is important: the subset residual [variance](../../../../../variance-split.md) generally includes omitted-variable bias.

For a finite candidate collection, choose a model minimizing $\widehat R(M)$, breaking ties in favour of a smaller model. The term $-n\widehat\sigma^2$ is common to all models, so this amounts to minimizing

$$
\operatorname{RSS}(M)+2k\widehat\sigma^2,
$$

the [Mallows Cp](../../../../../mallows-s-cp.md) form. The fit improvement competes with an increasing dimension penalty. Unbiasedness holds for each fixed model; the estimate at the data-selected model need not remain unbiased, because selection favours downward fluctuations. The method is a heuristic [model selection](../../../../../model-selection.md) rule, rather than an assertion that it finds the true model with certainty.

The printed $p\leq n$ includes a genuine qualification. If $p=n$, there are no full-model [residual degrees of freedom](../../../../../residual-degrees-of-freedom.md). Except in the balanced case $2k=n$, **no integrable data-only unbiased estimator can satisfy the requested identity for all means and unknown [variances](../../../../../variance-split.md)**. Here is a proof of the [unknown-variance risk estimation in a saturated Gaussian model](../../../../../unknown-variance-risk-estimation-in-a-saturated-gaussian-model.md) obstruction. Since $X$ is invertible, $\mu$ ranges over all $\mathbb R^n$. Suppose $T(Y)$ had the required expectation at every $\mu$ and [variance](../../../../../variance-split.md) $s>0$. For $v>0$, let $U\sim N_n(\mu,vI)$ and let $Y\mid U\sim N_n(U,sI)$. Marginally $Y\sim N_n(\mu,(s+v)I)$. Applying the assumed identity conditionally gives

$$
\mathbb ET(Y)=\mathbb E\|(I-P_M)U\|^2+ks=\|b_M\|^2+(n-k)v+ks,
$$

whereas applying it to the marginal distribution gives $\|b_M\|^2+k(s+v)$. Their difference is $(n-2k)v$, which must vanish. Integrability under the marginal Gaussian justifies conditioning. If $2k=n$, the obstruction disappears and the [residual sum of squares](../../../../../residual-sum-of-squares.md) alone has expectation $\|b_M\|^2+k\sigma^2$. Thus

$$
\boxed{p=n:\quad\widehat R(M)=\operatorname{RSS}(M)\text{ is unbiased exactly in the case }2k=n.}
$$

The general construction therefore requires $p<n$, or an independently available unbiased [variance](../../../../../variance-split.md) estimate.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

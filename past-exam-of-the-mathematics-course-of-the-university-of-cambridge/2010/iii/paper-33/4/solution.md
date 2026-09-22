<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

An unordered [bootstrap sample](../../../../../bootstrap-sample.md) is determined by the multiplicities $N_i\ge0$ of the $n$ distinct observations, with $\sum_iN_i=n$. Conversely each such vector specifies exactly one sample up to rearrangement. Place $n$ identical marks into $n$ boxes using $n-1$ separators. The [stars and bars](../../../../../stars-and-bars-combinatorics.md) argument therefore gives

$$
\boxed{\#\{\text{unordered bootstrap samples}\}=\binom{2n-1}{n-1}=\binom{2n-1}{n}.}
$$

These [bootstrap count vectors](../../../../../bootstrap-count-vectors.md) are not equally likely: the [probability](../../../../../probability.md) of a vector is $n!/(n^n\prod_iN_i!)$, counting its possible ordered sequences. The ordered index sequences themselves number $n^n$.

The first simulation uses independent standard [Cauchy distributions](../../../../../cauchy-distribution.md) and returns

$$
\widehat\theta=\frac1n\sum_{i=1}^n\mathbf1_{\{X_i>2\}}.
$$

The tail [probability](../../../../../probability.md) and [estimator](../../../../../estimator.md) moments are

$$
\theta=\frac12-\frac{\arctan2}{\pi}=\frac{\arctan(1/2)}\pi\approx0.1475836,
$$



$$
\boxed{\mathbb E\widehat\theta=\theta,\qquad
\operatorname{Var}(\widehat\theta)=\frac{\theta(1-\theta)}n.}
$$

The indicator count has a [binomial distribution](../../../../../binomial-distribution.md) with parameters $n,\theta$; the infinite [variance](../../../../../variance-split.md) of a Cauchy observation is irrelevant because this [estimator](../../../../../estimator.md) averages bounded indicators.

For the next code block, each row is an independent sample of size $n$ from the [empirical distribution](../../../../../type-information-theory.md) of the original $x_i$. Its entry in the vector $v$ is the corresponding bootstrap indicator mean $\widehat\theta_b^*$. The last expression is the [variance](../../../../../variance-split.md) of these $B=199$ replicate estimates, with denominator $B-1$:

$$
\widehat V_{\mathrm{boot}}=\frac1{B-1}\sum_{b=1}^B
(\widehat\theta_b^*-\overline{\widehat\theta^*})^2.
$$

Condition on the original data and write a star on bootstrap expectations. Every resampled indicator has a [Bernoulli distribution](../../../../../bernoulli-distribution.md) with success [probability](../../../../../probability.md) $\widehat\theta$, and the $n$ draws within a row are independent. Thus the [conditional bootstrap variance of a sample mean](../../../../../conditional-bootstrap-variance-of-a-sample-mean.md) gives

$$
\boxed{\mathbb E_*\widehat V_{\mathrm{boot}}=
\operatorname{Var}_*(\widehat\theta^*)=
\frac{\widehat\theta(1-\widehat\theta)}n.}
$$

It estimates the sampling [variance](../../../../../variance-split.md) of the tail-probability [estimator](../../../../../estimator.md), not the [variance](../../../../../variance-split.md) of the raw Cauchy data. Its square root is an estimated standard error. Finite $B$ leaves bootstrap simulation noise. Averaging over the original data, its expectation is $(n-1)\theta(1-\theta)/n^2$, so it is not exactly unbiased for the true [variance](../../../../../variance-split.md) $\theta(1-\theta)/n$ at finite $n$.

In the importance-sampling block, the transformation $Y=2/(1-U)$ gives, for $y\ge2$,

$$
\mathbb P(Y\le y)=1-\frac2y,\qquad q(y)=\frac2{y^2}\mathbf1_{\{y\ge2\}}.
$$

The variable $Y$ is a proposal draw supported entirely in the integration region. The deterministic value computed from it is the [importance sampling](../../../../../importance-sampling.md) weight

$$
W=\frac{f(Y)}{q(Y)}=\frac{Y^2}{2\pi(1+Y^2)}.
$$

Consequently

$$
\boxed{\widetilde\theta=\frac1n\sum_{i=1}^nW_i,\qquad
\mathbb E\widetilde\theta=\int_2^\infty\frac{f(y)}{q(y)}q(y)\,dy=\theta.}
$$

The code uses ordinary [importance sampling of a Cauchy tail](../../../../../importance-sampling-of-a-cauchy-tail.md), not self-normalization; $Y$ itself is neither an observation from the target Cauchy law nor the [estimator](../../../../../estimator.md)'s summand. The weight compensates for sampling from its proposal law.

The final block bootstraps these same proposal observations $Y_i$ and recomputes the weight average in each row. Since $W$ is a deterministic function of $Y$, this is equivalent to resampling the observed weights $W_i$. If $\widetilde\theta_b^*$ denotes a replicate, the final output is its [sample variance](../../../../../sample-variance.md) over the $B$ replicates. Its [conditional expectation](../../../../../conditional-expectation.md) is

$$
\boxed{\operatorname{Var}_*(\widetilde\theta^*)=
\frac1{n^2}\sum_{i=1}^n(W_i-\widetilde\theta)^2.}
$$

Its expectation over the original proposal sample is $(n-1)\operatorname{Var}(W)/n^2$.

The [variance](../../../../../variance-split.md) reduction can be calculated, rather than inferred just from the appearance of the weights. Write $A=\arctan(1/2)$. Then

$$
\mathbb EW^2=\frac1{2\pi^2}\int_2^\infty\frac{y^2}{(1+y^2)^2}\,dy
=\frac{A+2/5}{4\pi^2},
$$

because an antiderivative of the integrand without its prefactor is $\tfrac12(\arctan y-y/(1+y^2))$. Hence

$$
\boxed{\operatorname{Var}(W)=\frac{(A+2/5)/4-A^2}{\pi^2}
\approx9.55253\times10^{-5}.}
$$

By comparison, $\theta(1-\theta)\approx0.125803$. For $n=100$ the true [estimator](../../../../../estimator.md) [variances](../../../../../variance-split.md) are approximately $9.55253\times10^{-7}$ and $1.25803\times10^{-3}$ respectively. The importance [estimator](../../../../../estimator.md) has about **1/1,317 of the indicator [estimator](../../../../../estimator.md)'s [variance](../../../../../variance-split.md)**, because all proposals land in the tail and the weights remain in the narrow interval $[2/(5\pi),1/(2\pi))$.

Thus the last bootstrap output should usually be much smaller than the first, and its expected value is smaller by the same [variance](../../../../../variance-split.md) ratio. This is not a deterministic ordering of two finite-run outputs: if all the original Cauchy draws happen to be at most two, the first bootstrap [variance](../../../../../variance-split.md) is zero, while unequal importance weights can still give a positive second [variance](../../../../../variance-split.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

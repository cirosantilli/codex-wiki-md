<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Put $P=I-p^{-1}1_p1_p^T$, $Z=PX=X-\bar X1_p$, $Q=\|Z\|^2$ and $a=p-3$. Componentwise,

$$
\widehat\theta_j=X_j-\frac aQ(X_j-\bar X),\qquad\frac1p\sum_j\widehat\theta_j=\bar X.
$$

Thus the [James–Stein shrinkage toward the sample mean](../../../../../james-stein-shrinkage-toward-the-sample-mean.md) leaves the average unchanged and multiplies every contrast about it by the same data-dependent factor $1-a/Q$. If $Q>a$ the contrasts shrink without changing sign; if $Q<a$ their signs reverse, and if $Q<a/2$ their magnitudes increase. The event $Q=0$ has probability zero, and the estimator can be assigned $\bar X1_p$ there.

The [sample mean](../../../../../sample-mean.md) is a linear normal statistic with mean $\bar\theta$ and [variance](../../../../../variance-split.md) $1/p$, so

$$
\boxed{\bar X\sim N(\bar\theta,1/p).}
$$

The error splits into orthogonal mean and contrast components:

$$
\widehat\theta-\theta=(\bar X-\bar\theta)1_p+\left(1-\frac aQ\right)Z-P\theta.
$$

Since the second term is perpendicular to $1_p$, its cross product with the first is zero for every sample. Taking squared [norms](../../../../../norm.md) and expectations, $p\mathbb E(\bar X-\bar\theta)^2=1$, which yields the [risk function](../../../../../risk-function.md)

$$
\boxed{R(\widehat\theta,\theta)=1+\mathbb E_\theta\left\|\left(1-\frac aQ\right)Z-P\theta\right\|^2.}
$$

To compute the contrast risk, choose an [orthonormal basis](../../../../../orthonormal-basis.md) matrix $U$ for the range of $P$, with $U^TU=I_m$, $UU^T=P$ and $m=p-1\geq3$. Then $W=U^TX\sim N_m(\eta,I)$ with $\eta=U^T\theta$, $Q=\|W\|^2$, and the contrast [norm](../../../../../norm.md) is the [norm](../../../../../norm.md) of $(1-a/Q)W-\eta$. Expand it:

$$
\mathbb E_\theta\left\|\left(1-\frac aQ\right)W-\eta\right\|^2=m-2a\sum_{j=1}^m\mathbb E\frac{(W_j-\eta_j)W_j}{Q}+a^2\mathbb E\frac1Q.
$$

For $g_j(w)=w_j/\|w\|^2$, the [Gaussian Stein identity](../../../../../stein-s-lemma-probability.md) gives

$$
\mathbb E[(W_j-\eta_j)g_j(W)]=\mathbb E\partial_jg_j(W),\qquad\sum_{j=1}^m\partial_jg_j(w)=\frac{m-2}{\|w\|^2}.
$$

This application at a singularity is valid: near zero the reciprocal squared radius is integrable in dimension $m>2$, since its radial integral is $\int_0^1r^{m-3}dr$. Apply [Gaussian integration by parts](../../../../../stein-s-lemma-probability.md) outside a ball of radius $\varepsilon$; the inner boundary contribution is bounded by a constant times $\varepsilon^{m-2}$ and vanishes. The Gaussian tail eliminates the boundary at infinity. Therefore all required expectations are finite and the displayed identity holds.

Since $a=m-2=p-3$, the [Stein risk identity](../../../../../stein-risk-identity-for-normal-mean-estimators.md) now gives contrast risk $m-a^2\mathbb E(1/Q)$. Adding the unit mean risk proves

$$
\boxed{R(\widehat\theta,\theta)=p-(p-3)^2\mathbb E_\theta\frac1{\|X-\bar X1_p\|^2}.}
$$

Finally $Q$ has the [noncentral chi-squared distribution](../../../../../noncentral-chi-squared-distribution.md) $\chi_m^2(\lambda)$ with $\lambda=\|P\theta\|^2$. To establish where its reciprocal expectation is largest, complete the square in the normal representation $Q=\|W\|^2$ to obtain its [Laplace transform](../../../../../laplace-transform.md):

$$
\mathbb Ee^{-tQ}=(1+2t)^{-m/2}\exp\!\left(-\frac{\lambda t}{1+2t}\right),\qquad t\geq0.
$$

Since $1/q=\int_0^\infty e^{-tq}dt$, the [Tonelli theorem](../../../../../tonelli-theorem.md) gives the [reciprocal moment of a noncentral chi-squared variable](../../../../../reciprocal-moment-of-a-noncentral-chi-squared-variable.md)

$$
\mathbb E\frac1Q=\int_0^\infty(1+2t)^{-m/2}\exp\!\left(-\frac{\lambda t}{1+2t}\right)dt.
$$

Its integrand is positive and strictly decreasing in $\lambda$ for every $t>0$. The expectation is therefore strictly largest at $\lambda=0$, where

$$
\mathbb E\frac1Q=\int_0^\infty(1+2t)^{-m/2}dt=\frac1{m-2}=\frac1{p-3}.
$$

Because this expectation is subtracted in the risk, the minimizing set is exactly $P\theta=0$, that is, all coordinates of $\theta$ equal. On this line the risk is $p-(p-3)=3$:

$$
\boxed{\operatorname*{argmin}_{\theta\in\mathbb R^p}R(\widehat\theta,\theta)=\{c1_p:c\in\mathbb R\},\qquad\min_\theta R(\widehat\theta,\theta)=3.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

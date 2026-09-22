<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For [independent](../../../../../independent-random-variables.md) identically distributed observations $Y_1,\ldots,Y_n$, the [likelihood function](../../../../../likelihood-function.md) and [log-likelihood](../../../../../log-likelihood.md) are

$$
L_n(\theta)=\prod_{i=1}^n f(Y_i,\theta),\qquad\ell_n(\theta)=\sum_{i=1}^n\log f(Y_i,\theta).
$$

A [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) is a measurable choice $\widehat\theta_n\in\operatorname{argmax}_{\theta\in\Theta}L_n(\theta)$, when a maximizer exists. It need not be unique. The one-observation [score function](../../../../../informant-function.md) is $s_\theta(y)=\nabla_\theta\log f(y,\theta)$, and the [Fisher information matrix](../../../../../fisher-information-matrix.md) is

$$
I(\theta)=\mathbb E_\theta[s_\theta(Y)s_\theta(Y)^T]=-\mathbb E_\theta[\nabla_\theta^2\log f(Y,\theta)].
$$

Under the regularity assumptions, differentiation beneath the integral gives $\mathbb E_\theta s_\theta=\nabla_\theta\int f=0$. Differentiating again gives the second information identity. [Independent](../../../../../independent-random-variables.md) observations have total [Fisher information](../../../../../fisher-information-matrix.md) $nI(\theta)$.

Assume fixed parameter dimension, an interior true parameter $\theta_0$, a [positive-definite matrix](../../../../../positive-definite-matrix.md) $I(\theta_0)$, the standard differentiability and integrability conditions, and [statistical consistency](../../../../../consistency-statistics.md) of $\widehat\theta_n$. Then the [asymptotic normality of a maximum likelihood estimator](../../../../../asymptotic-normality-of-a-maximum-likelihood-estimator.md) is

$$
\boxed{\sqrt n(\widehat\theta_n-\theta_0)\ \xrightarrow{d}\ N_p(0,I(\theta_0)^{-1}).}
$$

Here $I$ is the information per observation. Thus the leading [covariance matrix](../../../../../covariance-matrix.md) of the estimator itself is $I(\theta_0)^{-1}/n$.

To prove this, [statistical consistency](../../../../../consistency-statistics.md) places the estimator in an interior ball about $\theta_0$ with [probability](../../../../../probability.md) tending to one, where its [score function](../../../../../informant-function.md) vanishes. Write $d_n=\widehat\theta_n-\theta_0$ and use the [integral first-order Taylor formula for a vector map](../../../../../integral-first-order-taylor-formula-for-a-vector-map.md):

$$
0=\nabla\ell_n(\theta_0)+\left\{\int_0^1\nabla^2\ell_n(\theta_0+t d_n)\,dt\right\}d_n.
$$

This integral matrix is needed in a vector problem; one does not have to assert a common scalar mean-value point for every score component. Put

$$
J_n=-\frac1n\int_0^1\nabla^2\ell_n(\theta_0+t d_n)\,dt.
$$

The regular local [uniform law of large numbers](../../../../../uniform-law-of-large-numbers.md), [continuity](../../../../../continuous-function.md) of the expected [Hessian matrix](../../../../../hessian-matrix.md), and [statistical consistency](../../../../../consistency-statistics.md) give $J_n\xrightarrow{P}I(\theta_0)$. The [multivariate central limit theorem](../../../../../multivariate-central-limit-theorem.md) gives

$$
\frac1{\sqrt n}\nabla\ell_n(\theta_0)=\frac1{\sqrt n}\sum_{i=1}^n s_{\theta_0}(Y_i)\ \xrightarrow{d}\ N_p(0,I(\theta_0)).
$$

The limiting information matrix is nonsingular, so $J_n^{-1}\xrightarrow{P}I(\theta_0)^{-1}$. Solving the Taylor identity and applying the [Slutsky theorem](../../../../../slutsky-theorem.md) proves the displayed normal limit, since $I^{-1}II^{-1}=I^{-1}$. Boundary parameters or singular information are outside this regular theorem.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

# Paper 30

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_30.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_30.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

For [independent](../../../random-variable.md#independent-random-variables) identically distributed observations $Y_1,\ldots,Y_n$, the [likelihood function](../../../statistical-modelling.md#likelihood-function) and [log-likelihood](../../../statistical-modelling.md#log-likelihood) are

$$
L_n(\theta)=\prod_{i=1}^n f(Y_i,\theta),\qquad\ell_n(\theta)=\sum_{i=1}^n\log f(Y_i,\theta).
$$

A [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator) is a measurable choice $\widehat\theta_n\in\operatorname{argmax}_{\theta\in\Theta}L_n(\theta)$, when a maximizer exists. It need not be unique. The one-observation [score function](../../../statistical-modelling.md#informant-function) is $s_\theta(y)=\nabla_\theta\log f(y,\theta)$, and the [Fisher information matrix](../../../statistical-modelling.md#fisher-information-matrix) is

$$
I(\theta)=\mathbb E_\theta[s_\theta(Y)s_\theta(Y)^T]=-\mathbb E_\theta[\nabla_\theta^2\log f(Y,\theta)].
$$

Under the regularity assumptions, differentiation beneath the integral gives $\mathbb E_\theta s_\theta=\nabla_\theta\int f=0$. Differentiating again gives the second information identity. [Independent](../../../random-variable.md#independent-random-variables) observations have total [Fisher information](../../../statistical-modelling.md#fisher-information-matrix) $nI(\theta)$.

Assume fixed parameter dimension, an interior true parameter $\theta_0$, a [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix) $I(\theta_0)$, the standard differentiability and integrability conditions, and [statistical consistency](../../../statistical-inference.md#consistency-statistics) of $\widehat\theta_n$. Then the [asymptotic normality of a maximum likelihood estimator](../../../statistical-modelling.md#asymptotic-normality-of-a-maximum-likelihood-estimator) is

$$
\boxed{\sqrt n(\widehat\theta_n-\theta_0)\ \xrightarrow{d}\ N_p(0,I(\theta_0)^{-1}).}
$$

Here $I$ is the information per observation. Thus the leading [covariance matrix](../../../variance.md#covariance-matrix) of the estimator itself is $I(\theta_0)^{-1}/n$.

To prove this, [statistical consistency](../../../statistical-inference.md#consistency-statistics) places the estimator in an interior ball about $\theta_0$ with [probability](../../../probability-theory.md#probability) tending to one, where its [score function](../../../statistical-modelling.md#informant-function) vanishes. Write $d_n=\widehat\theta_n-\theta_0$ and use the [integral first-order Taylor formula for a vector map](../../../calculus.md#integral-first-order-taylor-formula-for-a-vector-map):

$$
0=\nabla\ell_n(\theta_0)+\left\{\int_0^1\nabla^2\ell_n(\theta_0+t d_n)\,dt\right\}d_n.
$$

This integral matrix is needed in a vector problem; one does not have to assert a common scalar mean-value point for every score component. Put

$$
J_n=-\frac1n\int_0^1\nabla^2\ell_n(\theta_0+t d_n)\,dt.
$$

The regular local [uniform law of large numbers](../../../convergence-of-random-variables.md#uniform-law-of-large-numbers), [continuity](../../../calculus.md#continuous-function) of the expected [Hessian matrix](../../../calculus.md#hessian-matrix), and [statistical consistency](../../../statistical-inference.md#consistency-statistics) give $J_n\xrightarrow{P}I(\theta_0)$. The [multivariate central limit theorem](../../../convergence-of-random-variables.md#multivariate-central-limit-theorem) gives

$$
\frac1{\sqrt n}\nabla\ell_n(\theta_0)=\frac1{\sqrt n}\sum_{i=1}^n s_{\theta_0}(Y_i)\ \xrightarrow{d}\ N_p(0,I(\theta_0)).
$$

The limiting information matrix is nonsingular, so $J_n^{-1}\xrightarrow{P}I(\theta_0)^{-1}$. Solving the Taylor identity and applying the [Slutsky theorem](../../../statistical-inference.md#slutsky-theorem) proves the displayed normal limit, since $I^{-1}II^{-1}=I^{-1}$. Boundary parameters or singular information are outside this regular theorem.

## 2

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Represent the subset model by a set $M$ of $k$ column indices and let $X_M$ contain those columns. Its [ordinary least squares](../../../statistical-modelling.md#ordinary-least-squares) estimator sets the omitted coefficients to zero and has

$$
\widehat\theta_M=(X_M^TX_M)^{-1}X_M^TY,\qquad X\widehat\theta^M=P_MY,\qquad P_M=X_M(X_M^TX_M)^{-1}X_M^T.
$$

For $k=0$, use $P_M=0$. [Full column rank](../../../vector-space.md#full-column-rank) of $X$ implies [full column rank](../../../vector-space.md#full-column-rank) for each $X_M$. The matrix $P_M$ is an [orthogonal projection matrix](../../../linear-algebra.md#orthogonal-projection-matrix) of rank $k$.

Put $\mu=X\theta$ and $b_M=(I-P_M)\mu$. Projection [orthogonality](../../../linear-algebra.md#orthogonal-vectors) gives the [bias-variance decomposition of mean squared error](../../../statistical-modelling.md#bias-variance-decomposition-of-mean-squared-error)

$$
R(M)=\mathbb E\|P_MY-\mu\|^2=\|b_M\|^2+k\sigma^2,
$$

while the expected [residual sum of squares](../../../linear-regression.md#residual-sum-of-squares) is

$$
\mathbb E\|(I-P_M)Y\|^2=\|b_M\|^2+(n-k)\sigma^2.
$$

These equations distinguish the [mean-vector prediction risk](../../../statistical-inference.md#mean-vector-prediction-risk) in this problem from the additional noise in predicting a new response vector.

First take $p<n$. Let $P_X$ project onto the full column space of $X$. Since the full model contains $\mu$, the [residual estimate of Gaussian noise variance](../../../statistical-modelling.md#residual-estimate-of-gaussian-noise-variance)

$$
\widehat\sigma^2=\frac{\|(I-P_X)Y\|^2}{n-p}
$$

is unbiased: its numerator has expectation $(n-p)\sigma^2$. Consequently an [unbiased Gaussian projection risk estimate](../../../statistical-inference.md#unbiased-gaussian-projection-risk-estimate) is

$$
\boxed{\widehat R(M)=\|(I-P_M)Y\|^2+(2k-n)\widehat\sigma^2.}
$$

Indeed its expectation is $\|b_M\|^2+(n-k)\sigma^2+(2k-n)\sigma^2=R(M)$ for every $\theta$, even when the subset model omits true effects. [Independence](../../../random-variable.md#independent-random-variables) of the two terms is not needed for this expectation calculation. The full-model [variance](../../../variance.md) estimate is important: the subset residual [variance](../../../variance.md) generally includes omitted-variable bias.

For a finite candidate collection, choose a model minimizing $\widehat R(M)$, breaking ties in favour of a smaller model. The term $-n\widehat\sigma^2$ is common to all models, so this amounts to minimizing

$$
\operatorname{RSS}(M)+2k\widehat\sigma^2,
$$

the [Mallows Cp](../../../statistical-modelling.md#mallows-s-cp) form. The fit improvement competes with an increasing dimension penalty. Unbiasedness holds for each fixed model; the estimate at the data-selected model need not remain unbiased, because selection favours downward fluctuations. The method is a heuristic [model selection](../../../statistical-modelling.md#model-selection) rule, rather than an assertion that it finds the true model with certainty.

The printed $p\leq n$ includes a genuine qualification. If $p=n$, there are no full-model [residual degrees of freedom](../../../statistical-modelling.md#residual-degrees-of-freedom). Except in the balanced case $2k=n$, **no integrable data-only unbiased estimator can satisfy the requested identity for all means and unknown [variances](../../../variance.md)**. Here is a proof of the [unknown-variance risk estimation in a saturated Gaussian model](../../../statistical-inference.md#unknown-variance-risk-estimation-in-a-saturated-gaussian-model) obstruction. Since $X$ is invertible, $\mu$ ranges over all $\mathbb R^n$. Suppose $T(Y)$ had the required expectation at every $\mu$ and [variance](../../../variance.md) $s>0$. For $v>0$, let $U\sim N_n(\mu,vI)$ and let $Y\mid U\sim N_n(U,sI)$. Marginally $Y\sim N_n(\mu,(s+v)I)$. Applying the assumed identity conditionally gives

$$
\mathbb ET(Y)=\mathbb E\|(I-P_M)U\|^2+ks=\|b_M\|^2+(n-k)v+ks,
$$

whereas applying it to the marginal distribution gives $\|b_M\|^2+k(s+v)$. Their difference is $(n-2k)v$, which must vanish. Integrability under the marginal Gaussian justifies conditioning. If $2k=n$, the obstruction disappears and the [residual sum of squares](../../../linear-regression.md#residual-sum-of-squares) alone has expectation $\|b_M\|^2+k\sigma^2$. Thus

$$
\boxed{p=n:\quad\widehat R(M)=\operatorname{RSS}(M)\text{ is unbiased exactly in the case }2k=n.}
$$

The general construction therefore requires $p<n$, or an independently available unbiased [variance](../../../variance.md) estimate.

## 3

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The ordinary column [Gram matrix](../../../linear-algebra.md#gram-matrix) is $G=X^TX$. Use the normalized empirical [Gram matrix](../../../linear-algebra.md#gram-matrix)

$$
\widehat\Sigma=\frac1nX^TX,
$$

so that standard Gaussian entries give $\mathbb E\widehat\Sigma=I_p$. This is the normalization needed for concentration around $\|\theta\|_2^2$.

The [restricted isometry property](../../../numerical-analysis.md#restricted-isometry-property) of order $s$ with constant $0\leq\delta<1$ means that the normalized map $X/\sqrt n$ approximately preserves the [Euclidean norm](../../../functional-analysis.md#euclidean-norm) of all vectors with at most $s$ nonzero coordinates:

$$
(1-\delta)\|u\|_2^2\leq\frac1n\|Xu\|_2^2\leq(1+\delta)\|u\|_2^2.
$$

Equivalently, every principal block $\widehat\Sigma_{MM}$ with $|M|\leq s$ satisfies $\|\widehat\Sigma_{MM}-I\|_{\mathrm{op}}\leq\delta$. The least such $\delta$ is its [restricted isometry constant](../../../numerical-analysis.md#restricted-isometry-constant). In the unnormalized definition apply this property to $X/\sqrt n$ itself.

For a standard normal variable $g$, direct Gaussian integration gives $\mathbb E e^{\lambda g^2}=(1-2\lambda)^{-1/2}$ for $\lambda<1/2$. [Independence](../../../random-variable.md#independent-random-variables) therefore yields the [moment-generating function of a chi-squared distribution](../../../probability-theory.md#moment-generating-function-of-a-chi-squared-distribution), centred here at its mean:

$$
\log\mathbb E e^{\lambda Z}=n\left(-\lambda-\tfrac12\log(1-2\lambda)\right)\leq\frac{n\lambda^2}{1-2\lambda},\qquad0\leq\lambda<\tfrac12.
$$

The inequality follows from $-\log(1-u)-u=\sum_{j\geq2}u^j/j\leq u^2/(2(1-u))$. For $t>0$, the [Chernoff bound](../../../probability-inequality.md#chernoff-bound) with $\lambda=t/(2(n+t))$ gives

$$
\Pr(Z\geq t)\leq\exp\left(-\lambda t+\frac{n\lambda^2}{1-2\lambda}\right)=\exp\left(-\frac{t^2}{4(n+t)}\right).
$$

At $t=0$ the trivial [probability](../../../probability-theory.md#probability) bound suffices. This proves the requested bound, with a stronger prefactor one.

For the lower tail, $\log(1+u)\geq u-u^2/2$ gives $\log\mathbb E e^{-\lambda Z}\leq n\lambda^2$ for $\lambda\geq0$. Taking $\lambda=t/(2n)$ yields $\Pr(Z\leq-t)\leq e^{-t^2/(4n)}$. Combining both tails gives the useful [chi-squared concentration inequality](../../../probability-theory.md#chi-squared-concentration-inequality)

$$
\boxed{\Pr(|Z|\geq t)\leq2\exp\left(-\frac{t^2}{4(n+t)}\right),\qquad t\geq0.}
$$

For $z\geq0$ set $t=4(\sqrt{nz}+z)$. A direct calculation shows

$$
t^2-4z(n+t)=12nz+16z\sqrt{nz}\geq0.
$$

Thus the exponent is at least $z$, proving

$$
\boxed{\Pr(Z\geq4(\sqrt{nz}+z))\leq2e^{-z}.}
$$

The same threshold bounds the two-sided tail.

Finally fix a deterministic $\theta$ and put $r=\|\theta\|_2$. If $r>0$, [independence](../../../random-variable.md#independent-random-variables) of the Gaussian rows gives $X_i\theta/r\sim N(0,1)$ independently. Therefore

$$
\theta^T\widehat\Sigma\theta=r^2\left(1+\frac Zn\right).
$$

The two-sided bound just proved supplies

$$
\boxed{\Pr\!\left(\left|\theta^T\widehat\Sigma\theta-\|\theta\|_2^2\right|>4\|\theta\|_2^2\left(\sqrt{\frac zn}+\frac zn\right)\right)\leq2e^{-z}.}
$$

For $r=0$ the [quadratic form](../../../linear-algebra.md#quadratic-form) is deterministically zero; the strict inequality makes the formula valid in that case too. When $r\leq1$, replacing the threshold by $4(\sqrt{z/n}+z/n)$ gives an absolute bound [independent](../../../random-variable.md#independent-random-variables) of $\theta$. In particular every fixed such direction concentrates at rate $n^{-1/2}$ for a fixed confidence level. The [restricted isometry property](../../../numerical-analysis.md#restricted-isometry-property) requires a simultaneous statement over sparse directions; this fixed-direction calculation alone is not that stronger assertion.

## 4

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let $\Delta_n=\sup_{\theta\in\Theta}|Q_n(\theta)-Q(\theta)|$. For any $\varepsilon>0$, the set

$$
F_\varepsilon=\{\theta\in\Theta:\|\theta-\theta_0\|\geq\varepsilon\}
$$

is [compact](../../../topology.md#compact-space). If it is empty there is nothing to prove. Otherwise [continuity](../../../calculus.md#continuous-function) and the unique minimum give a strictly positive separation gap

$$
d_\varepsilon=\min_{\theta\in F_\varepsilon}\{Q(\theta)-Q(\theta_0)\}>0.
$$

Take any measurable attained [minimizer](../../../analysis.md#global-minimizer) of $Q_n$. Its defining inequality gives

$$
Q(\widehat\theta_n)\leq Q_n(\widehat\theta_n)+\Delta_n\leq Q_n(\theta_0)+\Delta_n\leq Q(\theta_0)+2\Delta_n.
$$

Consequently

$$
\boxed{\Pr(\|\widehat\theta_n-\theta_0\|\geq\varepsilon)\leq\Pr(\Delta_n\geq d_\varepsilon/2)\longrightarrow0.}
$$

This proves [argmin consistency under uniform convergence in probability](../../../statistical-inference.md#argmin-consistency-under-uniform-convergence-in-probability). No [continuity](../../../calculus.md#continuous-function) of $Q_n$ is needed once the [minimizer](../../../analysis.md#global-minimizer) exists; compactness and [continuity](../../../calculus.md#continuous-function) concern the deterministic separation gap. The [uniform convergence in probability](../../../convergence-of-random-variables.md#uniform-convergence-in-probability) assumption controls all candidate parameters, including the random [minimizer](../../../analysis.md#global-minimizer).

For the [estimating equation](../../../statistical-inference.md#estimating-equation), fix $\varepsilon>0$ and put $a=\theta_0-\varepsilon$, $b=\theta_0+\varepsilon$. The prescribed signs make $\eta=\tfrac12\min\{-S(a),S(b)\}>0$. Pointwise [convergence in probability](../../../convergence-of-random-variables.md#convergence-in-probability) at just these two points implies

$$
\Pr(S_n(a)\geq0)\leq\Pr(|S_n(a)-S(a)|\geq\eta)\longrightarrow0,
$$

and similarly $\Pr(S_n(b)\leq0)\to0$. With [probability](../../../probability-theory.md#probability) tending to one, $S_n(a)<0<S_n(b)$. The [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) then gives a zero inside $(a,b)$, and uniqueness identifies it with $\widehat\theta_n$. Hence

$$
\boxed{\Pr(|\widehat\theta_n-\theta_0|\geq\varepsilon)\leq\Pr(S_n(a)\geq0)+\Pr(S_n(b)\leq0)\longrightarrow0.}
$$

This is [consistency of a uniquely bracketed zero](../../../statistical-inference.md#consistency-of-a-uniquely-bracketed-zero). It needs no monotonicity, no [continuity](../../../calculus.md#continuous-function) of the limit $S$, and no uniform convergence of the $S_n$. The bracket interval must lie in the domain of $S_n$: read literally, the printed sign condition for every positive $\varepsilon$ puts every real point into $\Theta$, so this requirement is satisfied. More generally it is enough to have an interval about $\theta_0$ and sign brackets arbitrarily close to it.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)

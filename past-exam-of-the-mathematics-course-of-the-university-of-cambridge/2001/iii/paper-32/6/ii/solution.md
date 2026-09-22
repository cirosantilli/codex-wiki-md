<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Consider a regular $d$-parameter [statistical model](../../../../../../statistical-model-split.md) for which the data can locally be expressed as $(v,a)$, where $v=\widehat\theta$ is the [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) and $a$ is a suitable exact or higher-order [ancillary statistic](../../../../../../ancillary-statistic.md). Write the [log-likelihood](../../../../../../log-likelihood.md) as $\ell(\theta;v,a)$, and let

$$
j(v;v,a)=-\left.\partial_\theta\partial_\theta^{\mathsf T}\ell(\theta;v,a)\right|_{\theta=v}
$$

be its fitted [observed information](../../../../../../observed-fisher-information.md). The [P-star approximation](../../../../../../p-star-approximation.md) to the conditional sampling density of $v$, given $a$, is

$$
\boxed{p^*(v\mid a;\theta)=c(\theta,a)
|j(v;v,a)|^{1/2}
\exp\{\ell(\theta;v,a)-\ell(v;v,a)\}.}
$$

The normalizing factor is independent of $v$ and is chosen so the density integrates to one over the feasible estimator coordinates. Its leading Gaussian value is $(2\pi)^{-d/2}$, but exact normalization can change it. Both the fitted likelihood and the fitted information vary with $v$; the observed dataset is not held fixed while integrating over this sampling coordinate.

To see the structure, expand the likelihood difference for $v$ close to $\theta$. Its leading term is minus one half of the information-weighted quadratic displacement, while $|j(v)|^{1/2}$ supplies the local density scale. This recovers the first-order [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) of an efficient [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md). The formula is invariant under smooth one-to-one parameter changes: at a likelihood maximum the score vanishes, so the Hessian transforms as a quadratic form. Its square-root determinant supplies exactly the [Jacobian determinant](../../../../../../jacobian-determinant.md) required for the estimator density to transform.

There is a direct derivation in a full regular [exponential family](../../../../../../exponential-family-split.md). Let $S$ be the [sufficient statistic](../../../../../../sufficient-statistic.md) for an independent sample, with likelihood

$$
\ell(\theta;s)=\theta^{\mathsf T}s-n\kappa(\theta)+\text{data term}.
$$

The maximum-likelihood equation is $s=n\nabla\kappa(v)$, and its derivative is $j(v)=n\kappa''(v)$. Applying a multivariate [saddlepoint density approximation](../../../../../../saddlepoint-density-approximation.md) to $S$ gives

$$
f_S(s;\theta)\simeq(2\pi)^{-d/2}|j(v)|^{-1/2}
\exp\{\ell(\theta;s)-\ell(v;s)\}.
$$

Changing variables from $s$ to $v$ multiplies by $|ds/dv|=|j(v)|$, producing the displayed P-star form. In more general models, ancillary conditioning supplies the relevant local sample coordinates; an ancillary is not an arbitrary extra statistic.

For an illustrative exact case, take an independent sample from an [exponential distribution](../../../../../../exponential-distribution.md) with mean $\theta$, so $v=\bar Y$. The fitted [observed information](../../../../../../observed-fisher-information.md) is $j(v)=n/v^2$, and

$$
\ell(\theta;v)-\ell(v;v)=n\log(v/\theta)-nv/\theta+n.
$$

Thus P-star has density shape $v^{n-1}\theta^{-n}e^{-nv/\theta}$. Normalizing gives

$$
p^*(v;\theta)=\frac{n^n}{\Gamma(n)\theta^n}v^{n-1}e^{-nv/\theta},\qquad v>0,
$$

which is exactly the [gamma distribution](../../../../../../gamma-distribution.md) sampling density of the mean. Here sample ratios provide ancillary coordinates and are independent of the mean.

In suitable regular models the unnormalized leading construction has relative error of order $n^{-1}$, and higher-order ancillary constructions with normalization can attain relative order $n^{-3/2}$. Such accuracy needs the stated smoothness and ancillary hypotheses; it is not a universal consequence of asymptotic normality. The exact scale-model example is likewise a special property, not a general identity. The formula is useful for refined conditional inference, score distributions, and nuisance-likelihood adjustments, including [modified profile likelihood](../../../../../../modified-profile-likelihood.md). It describes a sampling density of the estimator, rather than a posterior density of the parameter.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

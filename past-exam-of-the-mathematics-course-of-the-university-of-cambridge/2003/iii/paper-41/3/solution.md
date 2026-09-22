<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $a$ be a suitable [ancillary statistic](../../../../../ancillary-statistic.md) and assume the sample can locally be written in coordinates $(v,a)$, where $v=\widehat\theta$ is the scalar [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md). Ancillarity means the sampling law of $a$ does not involve $\theta$. For each hypothetical sample coordinate $v$, write $\ell(\theta;v,a)$ for its [log-likelihood](../../../../../log-likelihood.md), and

$$
j(v;v,a)=-\left.\frac{\partial^2\ell(\theta;v,a)}{\partial\theta^2}\right|_{\theta=v}>0.
$$

The [P-star approximation](../../../../../p-star-approximation.md) to the conditional density with respect to $dv$ is

$$
\boxed{p^*(v\mid a;\theta)=c(\theta,a)\,j(v;v,a)^{1/2}\exp\{\ell(\theta;v,a)-\ell(v;v,a)\}.}
$$

Here $c(\theta,a)$ is chosen so the integral over the admissible $v$ domain is one; its leading regular approximation is $(2\pi)^{-1/2}$. One must vary the data coordinate $v$ inside the fitted information and likelihood, not evaluate those factors once at the observed estimate and treat them as constant. The expression combines the likelihood-ratio shape with the local information-volume factor. A quadratic likelihood gives the usual normal approximation, while the full shape retains skewness and other higher-order effects.

The approximation is invariant under smooth one-to-one parameter transformations: at the fitted point the transformed [observed information](../../../../../observed-fisher-information.md) acquires the square of the coordinate Jacobian, so its square root supplies exactly the density Jacobian. Under regular smooth fixed-dimensional likelihood and ancillary conditions it is a higher-order conditional approximation, typically with relative error of order $n^{-1}$, and in suitable refined settings of order $n^{-3/2}$. These are not universal error guarantees for singular, boundary or arbitrary ancillary constructions. In important transformation models the normalized formula is exact. The normalizing factor may depend on $\theta,a$; treating it as a universal constant can itself lose higher-order accuracy.

For a concrete check, in the exponential-mean model of Question 1 the likelihood difference is $n\log(v/\theta)-nv/\theta+n$ and $j(v)=n/v^2$. The resulting [P-star density for an exponential mean](../../../../../p-star-density-for-an-exponential-mean.md) normalizes to

$$
p^*(v;\theta)=\frac{n^n}{\Gamma(n)\theta^n}v^{n-1}e^{-nv/\theta},\qquad v>0,
$$

which is exactly the density of $\bar Y$. This example demonstrates the importance of both the information factor and normalization; it does not prove exactness for every regular model.

For the score density, fix an evaluation parameter $\theta_0$, and define $u(v,a)=\partial_\theta\ell(\theta_0;v,a)$. On any locally monotone branch, let $v=v(u,a)$. The [ancillary-conditioned score density](../../../../../ancillary-conditioned-score-density.md) is obtained by an ordinary change of variable:

$$
\boxed{f_U(u\mid a;\theta)\approx\frac{p^*(v(u,a)\mid a;\theta)}{|\partial_vu(v(u,a),a)|}.}
$$

If several branches give the same score, sum their contributions. The sampling parameter $\theta$ and the score-evaluation parameter $\theta_0$ have been distinguished; for the score at the true parameter take $\theta_0=\theta$. The denominator is a data-coordinate derivative, not automatically $j(\theta_0)$.

For the conditional distribution function of the estimate, integrate the normalized density:

$$
\boxed{\mathbb P_\theta(\widehat\theta\leq v_0\mid a)\approx\frac{\int_{v\leq v_0}\sqrt{j(v;v,a)}\,e^{\ell(\theta;v,a)-\ell(v;v,a)}dv}{\int\sqrt{j(v;v,a)}\,e^{\ell(\theta;v,a)-\ell(v;v,a)}dv}.}
$$

Both integrals use the actual support and observed ancillary value. Numerical quadrature gives tail probabilities or confidence limits by inversion. Conditional inference should not silently average over the ancillary, because it is the conditional distribution that this construction is designed to approximate.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

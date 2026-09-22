<h1 id="5i/solution">Solution</h1>

↑ **Parent:** [5I](../5i.md)

The independent [Laplace distribution](../../../../../laplace-distribution.md) responses have log likelihood

$$
\ell(\beta,\sigma)=-n\log(2\sigma)-\frac{S_1(\beta)}\sigma.
$$

For every fixed positive $\sigma$, maximizing this expression means minimizing the sum of absolute residuals. Thus **$\widehat\beta$ is a [least absolute deviations](../../../../../laplace-regression.md) estimate**, not a least-squares estimate. Such a minimizer exists: minimize the distance in the finite-dimensional closed column space of the design matrix. It need not be unique if the data or design allow multiple minimizers.

Write $s=S_1(\widehat\beta)$. For $s>0$, differentiating the profiled log likelihood gives $-n/\sigma+s/\sigma^2=0$. Its unique maximum is

$$
\boxed{\widehat\sigma=\frac{S_1(\widehat\beta)}n.}
$$

If the fitted residual sum is zero, the likelihood instead increases without bound as $\sigma\downarrow0$: there is no joint maximum with the stated positive scale parameter. The displayed estimate then denotes the boundary limit, not an admissible positive-scale MLE.

An ordinary [exponential dispersion family](../../../../../exponential-dispersion-model.md) has log density $[y\theta-b(\theta)]/a(\sigma)+c(y,\sigma)$, so changing the mean changes the log density by an affine function of $y$. For two distinct Laplace locations $\mu_1,\mu_2$, their log-density difference is $(|y-\mu_2|-|y-\mu_1|)/\sigma$, with different slopes on the intervals separated by the two locations. It is not affine in $y$. Equivalently the kink at $y=\mu$ moves with the parameter. **The Laplace location family is not an ordinary [exponential dispersion family](../../../../../exponential-dispersion-model.md).**

## ↑ Ancestors (10)

1. [5I](../5i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

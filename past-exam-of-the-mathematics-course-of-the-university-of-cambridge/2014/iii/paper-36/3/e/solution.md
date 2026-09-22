<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Start from any $(a^{(0)},b^{(0)})$. For independent draws $G_{1,k},G_{2,k}$ from the [standard normal distribution](../../../../../../standard-normal-distribution.md) at each sweep, the [Gibbs sampler](../../../../../../gibbs-sampler.md) can be implemented as

$$
\boxed{a^{(k+1)}=\frac{r-Cb^{(k)}}A+\frac{G_{1,k}}{\sqrt A},\qquad
b^{(k+1)}=\frac{s-Ca^{(k+1)}}D+\frac{G_{2,k}}{\sqrt D}.}
$$

The second update must use the newly drawn first coordinate. The transform in part (a) supplies the needed independent Gaussian draws. Each conditional update preserves the joint [posterior](../../../../../../bayesian-posterior.md), so their composition does too.

Convergence is particularly transparent here. Centering at the [posterior](../../../../../../bayesian-posterior.md) mean gives

$$
b^{(k+1)}-\mu_b=\frac{C^2}{AD}(b^{(k)}-\mu_b)-\frac{C}{D\sqrt A}G_{1,k}+\frac{G_{2,k}}{\sqrt D}.
$$

Positive definiteness gives $C^2/(AD)<1$, so this is a stable Gaussian autoregression. The full sampler has the desired [posterior](../../../../../../bayesian-posterior.md) as its limiting invariant law. This is the [linear contraction of a two-coordinate Gaussian Gibbs sweep](../../../../../../linear-contraction-of-a-two-coordinate-gaussian-gibbs-sweep.md).

For a [posterior](../../../../../../bayesian-posterior.md)-integrable function $\phi$, its [posterior](../../../../../../bayesian-posterior.md) expectation is estimated after a burn-in $K$ by

$$
\boxed{\widehat{\mathbb E}_\pi\phi=\frac1L\sum_{k=K+1}^{K+L}\phi(a^{(k)},b^{(k)}).}
$$

The ergodic theorem justifies this Monte Carlo average. The retained values of $\phi$ also approximate its [posterior](../../../../../../bayesian-posterior.md) distribution and quantiles. If a Bayesian point estimate is requested under squared-error loss, the [posterior](../../../../../../bayesian-posterior.md) mean is the appropriate estimate, when its needed moments exist. An arbitrary function need not have a finite [posterior](../../../../../../bayesian-posterior.md) mean; integrability must be assumed for the displayed target. Successive Gibbs draws are correlated, so uncertainty in the Monte Carlo average should use chain-aware error estimates rather than treating them as iid.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

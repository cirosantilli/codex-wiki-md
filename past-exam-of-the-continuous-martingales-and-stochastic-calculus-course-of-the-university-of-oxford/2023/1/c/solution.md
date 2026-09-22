<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For any real [orthonormal basis](../../../../orthonormal-basis.md) $(G_i)$, the argument of (b)(ii) gives [almost sure convergence](../../../../almost-sure-convergence.md) and [convergence in L2](../../../../convergence-in-l2.md) of $\widetilde Wh$. Finite linear combinations have [normal distributions](../../../../normal-distribution.md), and the [Parseval identity for a Hilbertian basis](../../../../parseval-identity-for-a-hilbertian-basis.md) gives

$$
\mathbb E[(\widetilde Wf)(\widetilde Wg)]=\sum_i\langle f,G_i\rangle\langle g,G_i\rangle
=\langle f,g\rangle.
$$

Thus $W$ and $\widetilde W$ are centered [Gaussian processes](../../../../gaussian-process-split.md) with the same [covariance function](../../../../covariance-function.md). More explicitly, their finite-dimensional [characteristic functions](../../../../characteristic-function-split.md) are both

$$
\boxed{\mathbb E\exp\!\left(i\sum_{j=1}^mu_jWh_j\right)
=\exp\!\left(-\frac12\left\|\sum_{j=1}^mu_jh_j\right\|_{\mathcal H}^2\right).}
$$

This proves the [basis invariance of an isonormal Gaussian process](../../../../basis-invariance-of-an-isonormal-gaussian-process.md): equality of all [finite-dimensional distributions](../../../../finite-dimensional-distribution.md), and hence equality in law of the indexed collections.

For the specified cosine [orthonormal basis](../../../../orthonormal-basis.md), put $\lambda_i=\pi(i-\tfrac12)$. Its coefficient against an interval indicator is

$$
\langle\mathbf1_{[0,t]},G_i\rangle
=\sqrt2\int_0^t\cos(\lambda_i s)\,ds
=\frac{\sqrt2\sin(\lambda_i t)}{\lambda_i}.
$$

Consequently the [Brownian half-integer sine expansion](../../../../brownian-half-integer-sine-expansion.md), a [Karhunen–Loève expansion](../../../../karhunen-loeve-expansion.md), is

$$
\boxed{\widetilde B_t
=\sqrt2\sum_{i=1}^\infty b_i\frac{\sin(\pi(i-\tfrac12)t)}{\pi(i-\tfrac12)}.}
$$

For every fixed $t$, the sum converges [almost surely](../../../../almost-sure-convergence.md) and in [L2 space](../../../../l2-space-is-a-hilbert-space.md) because the coefficient squares sum to $\|\mathbf1_{[0,t]}\|^2=t$. Its [continuous modification](../../../../continuous-modification.md) is a standard [Brownian motion](../../../../brownian-motion-split.md) by (b)(v). The expansion also holds in $L^2(\Omega\times[0,1])$: the [expectation](../../../../expected-value-split.md) of the squared tail is the integral of the coefficient-square tail, which tends to zero by the [dominated convergence theorem](../../../../dominated-convergence-theorem.md), with bound $t$.

To realize this expansion for the original $B$, choose $b_i=WG_i$. These are [Jointly Gaussian](../../../../multivariate-normal-distribution.md) with [covariance matrix](../../../../covariance-matrix.md) equal to the identity, hence are [independent](../../../../independent-random-variables.md) [standard normal random variables](../../../../standard-normal-random-variable.md). The finite [orthogonal projections](../../../../orthogonal-projection.md) of $\mathbf1_{[0,t]}$ onto $G_1,\ldots,G_N$ converge in $\mathcal H$, and the identity $\mathbb E|Wh|^2=\|h\|^2$ transfers that convergence to the displayed expansion for $B_t$. With an independently chosen sequence $(b_i)$ the resulting [Brownian motion](../../../../brownian-motion-split.md) has the same law; a pathwise identification uses the coupling just given.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the continuous martingales and stochastic calculus course of the University of Oxford](../../../split.md)
5. [Continuous martingales and stochastic calculus course of the University of Oxford](../../../../continuous-martingales-and-stochastic-calculus-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

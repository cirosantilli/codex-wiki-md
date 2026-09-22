<h1 id="28k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For observation $X=k$, the likelihood is proportional to $p^k(1-p)^{n-k}$. For $0<k<n$, its logarithmic [derivative](../../../../../../derivative.md) is $k/p-(n-k)/(1-p)$, vanishing uniquely at $k/n$; the logarithm is strictly concave. At $k=0$ or $k=n$, monotonicity gives the boundary maximum. Thus the [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) is

$$
\boxed{\widehat p_{\rm ML}=X/n}.
$$

A [uniform prior](../../../../../../uniform-prior.md) multiplies this likelihood by a constant. The beta-integral normalization therefore gives the [posterior distribution](../../../../../../bayesian-posterior.md)

$$
\boxed{p\mid X=k\sim\operatorname{Beta}(k+1,n-k+1)}.
$$

In particular the posterior mean $(k+1)/(n+2)$ is not automatically the optimal estimator for the weighted loss in the next part.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [28K](../../28k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

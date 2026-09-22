<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [natural exponential family](../../../../../../natural-exponential-family.md) of order $p$ has an observation vector $Y\in\mathbb R^p$ and [probability density function](../../../../../../probability-density-function.md), relative to a fixed reference measure $\nu$,

$$
f_\theta(y)=h(y)\exp\{\theta^Ty-\kappa(\theta)\},\qquad \kappa(\theta)=\log\int h(y)e^{\theta^Ty}\,d\nu(y).
$$

Its [natural parameter space](../../../../../../natural-parameter-space.md) is $\mathcal N=\{\theta\in\mathbb R^p:\kappa(\theta)<\infty\}$. A [full natural exponential family](../../../../../../full-natural-exponential-family.md) allows every $\theta\in\mathcal N$. A [regular natural exponential family](../../../../../../regular-natural-exponential-family.md) has an open parameter space; fullness and regularity together mean that $\mathcal N$ itself is open. A [minimal exponential family](../../../../../../minimal-exponential-family.md) additionally requires that no nonzero [linear combination](../../../../../../linear-combination.md) of the components of $Y$ be constant [almost surely](../../../../../../almost-sure-convergence.md). This is the condition that the genuinely needed number of canonical [sufficient statistics](../../../../../../sufficient-statistic.md) is $p$.

[Hölder's inequality](../../../../../../holder-s-inequality.md) shows that $\mathcal N$ is convex: for $0<t<1$, its normalizing integral at $t\theta+(1-t)\eta$ is at most the product of the respective integrals to powers $t$ and $1-t$. Taking logarithms also proves [convexity](../../../../../../convex-function.md) of the [cumulant function](../../../../../../cumulant-function-of-an-exponential-family.md) $\kappa$. In the minimal case its [Hessian matrix](../../../../../../hessian-matrix.md) is positive definite on the interior, as the [covariance](../../../../../../covariance.md) calculation below establishes. Keeping fullness, regularity and minimality separate matters when discussing existence or uniqueness of a [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $y_{(n)}=\max_i y_i$ and $c=\max(\beta,y_{(n)})$. For the observed positive data, the [uniform distribution](../../../../continuous-uniform-distribution.md) [likelihood function](../../../../likelihood-function.md) is

$$
L(\theta;y)=\theta^{-n}\mathbf1_{\{\theta>y_{(n)}\}}.
$$

Multiplying by the [Pareto distribution](../../../../pareto-distribution.md) [prior density](../../../../prior-density.md) gives the [posterior density](../../../../posterior-density.md) kernel $\theta^{-(\alpha+n+1)}\mathbf1_{\{\theta>c\}}$. Since

$$
\int_c^\infty\theta^{-(\alpha+n+1)}\,d\theta
=\frac{c^{-(\alpha+n)}}{\alpha+n},
$$

the normalized [posterior distribution](../../../../bayesian-posterior.md) is

$$
\boxed{\theta\mid y\sim\operatorname{Pareto}(\alpha+n,c),\qquad
\pi(\theta\mid y)=\frac{(\alpha+n)c^{\alpha+n}}{\theta^{\alpha+n+1}}\mathbf1_{\{\theta>c\}}.}
$$

This is [uniform-Pareto conjugacy](../../../../uniform-pareto-conjugacy.md). The [posterior density](../../../../posterior-density.md) is strictly decreasing over its support, so the [highest posterior density interval](../../../../highest-posterior-density-interval.md) starts at $c$, where the admissible density is largest in the limiting sense. Its upper endpoint $u$ satisfies

$$
\mathbb P(\theta>u\mid y)=\left(\frac cu\right)^{\alpha+n}=0.05.
$$

Hence a 95% [highest posterior density interval](../../../../highest-posterior-density-interval.md) is

$$
\boxed{\left(c,\;c\,20^{1/(\alpha+n)}\right),\qquad c=\max\!\left(\beta,\max_iY_i\right).}
$$

Inclusion of endpoints does not change its [posterior probability](../../../../posterior-probability.md). Every point inside has higher [posterior density](../../../../posterior-density.md) than every admissible point to its right, and points below $c$ have density zero. This is the [Pareto highest density interval](../../../../pareto-highest-density-interval.md); equal endpoint densities are unnecessary because one endpoint is the support boundary.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the statistics course of the University of Oxford](../../../split.md)
5. [Statistics course of the University of Oxford](../../../../statistics-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

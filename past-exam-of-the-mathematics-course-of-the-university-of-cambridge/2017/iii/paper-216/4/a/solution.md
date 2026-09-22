<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\pi(x)=\mu(x\mid y)$. [Mean-field variational inference](../../../../../../mean-field-variational-inference.md) minimizes the reverse [Kullback-Leibler divergence](../../../../../../kullback-leibler-divergence.md)

$$
\operatorname{KL}(q\Vert\pi)=\int q(x)\log\frac{q(x)}{\pi(x)}\,dx,
\qquad q(x)=\prod_{i=1}^pq_i(x_i),\quad \int q_i=1.
$$

Each $q_i$ is a [probability density function](../../../../../../probability-density-function.md); without further parametric restrictions, the optimization is over all such product [probability distributions](../../../../../../probability-distribution.md). Equivalently it maximizes the [evidence lower bound](../../../../../../evidence-lower-bound.md) $\mathbb E_q[\log h(X)-\log q(X)]$ for any unnormalized [posterior density](../../../../../../posterior-density.md) $h$. Its difference from $\log\int h$ is exactly the [Kullback-Leibler divergence](../../../../../../kullback-leibler-divergence.md).

Fix $q_2,\ldots,q_p$ and write

$$
F(x_1)=\mathbb E_{q_{-1}}[\log\pi(x_1,X_{-1})],\qquad
Z_1=\int e^{F(u)}\,du.
$$

Assume $0<Z_1<\infty$ and that the displayed [expected values](../../../../../../expected-value.md) and objective decomposition are well defined. The optimal factor is

$$
\boxed{q_1^*(x_1)=\frac{\exp\{\mathbb E_{q_{-1}}[\log\pi(x_1,X_{-1})]\}}{Z_1}.}
$$

Indeed, the part of the objective depending on $q_1$ is

$$
\int q_1\log q_1-\int q_1F
=\operatorname{KL}(q_1\Vert q_1^*)-\log Z_1.
$$

The remaining term $\sum_{i=2}^p\int q_i\log q_i$ is fixed. [Gibbs inequality](../../../../../../gibbs-inequality.md) gives nonnegativity of the [Kullback-Leibler divergence](../../../../../../kullback-leibler-divergence.md), with equality precisely at $q_1=q_1^*$ almost everywhere. This proves global optimality of that coordinate update; it does not assert global optimality of a sequence of coordinate updates for the full nonconvex product-family problem.

The printed upper index $k$ in the list of remaining coordinates is inconsistent with the dimension $p$; the natural interpretation is $k=p$. Also, if the exponential expression has zero or infinite [normalizing constant](../../../../../../normalizing-constant.md), or the [expected values](../../../../../../expected-value.md) are undefined, the usual coordinate formula needs additional support or integrability hypotheses. A restricted parametric factor family need not contain this unrestricted optimal factor.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

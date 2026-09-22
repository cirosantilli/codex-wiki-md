<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $a=(2,1)^T$, so the data map is $a^Tu$. The [Gaussian likelihood](../../../../../../gaussian-likelihood.md) and [prior distribution](../../../../../../prior-probability.md) give

$$
\pi^m(u)\propto\exp\left[-\frac12u^Tu-\frac{(m-a^Tu)^2}{2\delta^2}\right].
$$

[Completing the square](../../../../../../completing-the-square.md), or using [Gaussian conjugacy for a normal linear model](../../../../../../gaussian-conjugacy-for-a-normal-linear-model.md), identifies a [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) with [precision matrix](../../../../../../precision-matrix.md) $C_\delta^{-1}=I_2+\delta^{-2}aa^T$. Since $a^Ta=5$, its [posterior mean](../../../../../../posterior-mean.md) and [covariance matrix](../../../../../../covariance-matrix.md) are

$$
\boxed{u\mid m\sim\mathcal N(b_\delta,C_\delta).}
$$

The parameters are

$$
\begin{aligned}
b_\delta&=\frac{m}{5+\delta^2}\begin{pmatrix}2\\1\end{pmatrix},\\
C_\delta&=I_2-\frac{aa^T}{5+\delta^2}
=\frac1{5+\delta^2}\begin{pmatrix}1+\delta^2&-2\\-2&4+\delta^2\end{pmatrix}.
\end{aligned}
$$

For example, $(I_2+\delta^{-2}aa^T)C_\delta=I_2$, which checks the square completion.

The [orthogonal vectors](../../../../../../orthogonal-vectors.md)

$$
e_\parallel=\frac1{\sqrt5}(2,1)^T,\qquad
e_\perp=\frac1{\sqrt5}(-1,2)^T
$$

are [eigenvectors](../../../../../../eigenvector.md) of the [covariance matrix](../../../../../../covariance-matrix.md). Their respective [variances](../../../../../../variance-split.md) are

$$
\boxed{\operatorname{Var}(e_\parallel^Tu\mid m)=\frac{\delta^2}{5+\delta^2},\qquad
\operatorname{Var}(e_\perp^Tu\mid m)=1.}
$$

They are independent under the [posterior distribution](../../../../../../bayesian-posterior.md), by [independence of uncorrelated jointly normal variables](../../../../../../independence-of-uncorrelated-jointly-normal-variables.md). Thus uncertainty is different in the two directions even for positive noise: the data constrain $e_\parallel$, whereas $e_\perp$ spans the [null space](../../../../../../kernel-of-a-linear-map.md) of the data map.

As $\delta\to0$, the [posterior distribution](../../../../../../bayesian-posterior.md) converges to the law of

$$
\frac m5(2,1)^T+Ze_\perp,\qquad Z\sim\mathcal N(0,1).
$$

This is supported on $2u_1+u_2=m$, and its [posterior mean](../../../../../../posterior-mean.md) is the [minimum-norm least-squares solution](../../../../../../minimum-norm-least-squares-solution.md). The [prior distribution](../../../../../../prior-probability.md) still determines the distribution along the unobserved [null space](../../../../../../kernel-of-a-linear-map.md); it has not disappeared. This example of a [Gaussian posterior in the zero-noise limit](../../../../../../gaussian-posterior-in-the-zero-noise-limit.md) distinguishes exact recovery of an observed component from recovery of the whole unknown.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 350](../../../paper-350-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

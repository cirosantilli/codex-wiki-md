<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For $r>0$, let $\kappa_r$ be the [probability](../../../../../probability.md) law of a seed displacement from its tree. For the literal circular support, it is normalized [arclength](../../../../../arc-length.md) on $\{u:|u|=r\}$. The conditional [mean measure of a point process](../../../../../intensity-measure-of-a-point-process.md) is

$$
\boxed{\Lambda_\Pi(A)=\mu\sum_{z\in\Pi}\kappa_r(A-z).}
$$

We prove the conditional Poisson assertion directly by joint [probability generating functions](../../../../../probability-generating-function.md).

Fix disjoint bounded [measurable](../../../../../measurability.md) sets $A_1,\ldots,A_k$. For a tree at $z$, put $q_j(z)=\kappa_r(A_j-z)$ and $q_0(z)=1-\sum_jq_j(z)$. Conditional on its seed count, the allocation among these sets and their complement is [multinomial distribution](../../../../../multinomial-distribution.md). Averaging over the Poisson seed count gives

$$
\mathbb E\left[\prod_{j=1}^k s_j^{N_z(A_j)}\,\middle|\,\Pi\right]
=\exp\left[\mu\left(q_0(z)+\sum_jq_j(z)s_j-1\right)\right]
=\prod_{j=1}^k\exp\bigl(\mu q_j(z)(s_j-1)\bigr).
$$

Thus this tree contributes [independent](../../../../../independent-random-variables.md) Poisson counts of means $\mu q_j(z)$ to the disjoint sets. Different trees contribute independently. Only trees within distance $r$ of the bounded union of the $A_j$ can contribute, and there are [almost surely](../../../../../almost-sure-convergence.md) finitely many of them. Multiplying their [probability generating functions](../../../../../probability-generating-function.md) gives

$$
\mathbb E\left[\prod_j s_j^{\Pi^*(A_j)}\,\middle|\,\Pi\right]
=\prod_j\exp\bigl(\Lambda_\Pi(A_j)(s_j-1)\bigr).
$$

This is precisely the joint [probability generating function](../../../../../probability-generating-function.md) of [independent](../../../../../independent-random-variables.md) Poisson counts with the displayed means. Also $\Lambda_\Pi$ is locally finite, because each bounded set can receive seeds from only finitely many trees. This proves the conditional [Poisson point process](../../../../../poisson-point-process.md) assertion and the [Poisson offspring clusters directed by their parent process](../../../../../poisson-offspring-clusters-directed-by-their-parent-process.md) construction.

In [arclength](../../../../../arc-length.md) notation the directing measure is $\Lambda_\Pi=\mu\sum_{z\in\Pi}\sigma_{z,r}/(2\pi r)$, where $\sigma_{z,r}$ is [arclength](../../../../../arc-length.md) on the circle centered at $z$. If “circle” is used to mean the filled disc instead, take $\kappa_r(du)=\mathbf1_{\{|u|\le r\}}du/(\pi r^2)$; then

$$
\Lambda_\Pi(dx)=\frac{\mu}{\pi r^2}\sum_{z\in\Pi}\mathbf1_{\{|x-z|\le r\}}\,dx.
$$

The generating-function proof and the following unconditional conclusion hold for either reading. The circular version has a singular conditional directing measure, giving the [random directing measure of a Cox process](../../../../../random-directing-measure-of-a-cox-process.md) formulation.

Unconditionally this is a [Cox process](../../../../../cox-process.md), specifically a Poisson-offspring [Neyman-Scott process](../../../../../neyman-scott-process.md). Its [mean measure of a point process](../../../../../intensity-measure-of-a-point-process.md) is nevertheless spatially uniform. With $q_A(z)=\kappa_r(A-z)$, the [Campbell first-moment formula](../../../../../campbell-first-moment-formula.md) and translation invariance give

$$
\mathbb E\Lambda_\Pi(A)=\lambda\mu\int_{\mathbb R^2}q_A(z)\,dz
=\lambda\mu|A|,
$$

since $\int q_A(z)dz=\int\kappa_r(du)\int\mathbf1_A(z+u)dz=|A|$. Uniform mean alone does not establish a Poisson law.

For a bounded set $A$ of positive area, the conditional count has mean and [variance](../../../../../variance-split.md) $\Lambda_\Pi(A)$. The [law of total variance](../../../../../law-of-total-variance.md) gives

$$
\operatorname{Var}\Pi^*(A)=\mathbb E\Lambda_\Pi(A)+\operatorname{Var}\Lambda_\Pi(A).
$$

A Poisson integral of a deterministic function $q$ has [variance](../../../../../variance-split.md) $\lambda\int q^2dz$: for a simple function on disjoint sets this follows from [independent](../../../../../independent-random-variables.md) Poisson counts, and square-integrable approximation gives the general formula. Here $0\le q_A\le1$ and it has bounded support, so

$$
\boxed{\operatorname{Var}\Pi^*(A)
=\lambda\mu|A|+\lambda\mu^2\int_{\mathbb R^2}q_A(z)^2\,dz
>\lambda\mu|A|=\mathbb E\Pi^*(A).}
$$

The strict inequality holds when $\lambda,\mu>0$, because $\int q_A=|A|>0$ implies $\int q_A^2>0$. A Poisson [random variable](../../../../../random-variable-split.md) has equal mean and [variance](../../../../../variance-split.md). Hence **the unconditional process is not a [Poisson process](../../../../../poisson-process.md) in the nontrivial model**. If $\lambda=0$ or $\mu=0$, there are no seeds and the process is the degenerate empty [Poisson process](../../../../../poisson-process.md). The [overdispersion of nondegenerate mixed Poisson counts](../../../../../overdispersion-of-nondegenerate-mixed-poisson-counts.md) quantifies the additional clustering induced by the random parents.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

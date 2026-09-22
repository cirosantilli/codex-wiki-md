<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a cost $c:X\times Y\to[0,+\infty]$ that is a [Borel measurable function](../../../../../../borel-measurable-function.md), a [transport map](../../../../../../transport-map.md) is a measurable $T:X\to Y$ whose [pushforward measure](../../../../../../pushforward-measure.md) satisfies

$$
T_\#\mu=\nu,\qquad \mu(T^{-1}(B))=\nu(B)\quad\text{for every Borel }B\subseteq Y.
$$

The [Monge optimal transport problem](../../../../../../monge-optimal-transport-problem.md) moves every source point to one destination:

$$
\boxed{\inf_{T_\#\mu=\nu}\mathbb M(T),\qquad \mathbb M(T)=\int_X c(x,T(x))\,d\mu(x).}
$$

The [Kantorovich optimal transport problem](../../../../../../kantorovich-optimal-transport-problem.md) permits mass to split. Its admissible [transport plans](../../../../../../transport-plan.md) are the [probability measures](../../../../../../probability-measure.md) on $X\times Y$ with prescribed [marginal distributions](../../../../../../marginal-distribution.md):

$$
\Pi(\mu,\nu)=\{\pi:(p_X)_\#\pi=\mu,\ (p_Y)_\#\pi=\nu\},\qquad
\boxed{\inf_{\pi\in\Pi(\mu,\nu)}\mathbb K(\pi),\quad \mathbb K(\pi)=\int_{X\times Y}c\,d\pi.}
$$

Thus a [transport plan](../../../../../../transport-plan.md) is a [coupling of probability distributions](../../../../../../coupling.md). The set $\Pi(\mu,\nu)$ is never empty: it contains the [product measure](../../../../../../product-measure.md) $\mu\otimes\nu$. Signed costs can also be used when their integrals are well defined, for example with an integrable lower bound of the form $a(x)+b(y)$.

On the [Polish space](../../../../../../polish-space.md) $\mathbb R$, take the [Dirac measures](../../../../../../dirac-measure.md)

$$
\boxed{\mu=\delta_0,\qquad \nu=\tfrac12\delta_{-1}+\tfrac12\delta_1.}
$$

Every measurable map satisfies $T_\#\delta_0=\delta_{T(0)}$, which cannot equal $\nu$. A [transport map](../../../../../../transport-map.md) cannot split an [atom of a measure](../../../../../../atom-measure-theory.md), whereas the [transport plan](../../../../../../transport-plan.md) $\tfrac12\delta_{(0,-1)}+\tfrac12\delta_{(0,1)}$ can.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 348](../../../paper-348-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

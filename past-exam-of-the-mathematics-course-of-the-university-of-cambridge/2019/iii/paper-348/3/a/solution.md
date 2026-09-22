<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The dual of the [Kantorovich optimal transport problem](../../../../../../kantorovich-optimal-transport-problem.md) is

$$
\boxed{\sup_{(u,v)\in\mathcal A_c}\left\{\int_Xu\,d\mu+\int_Yv\,d\nu\right\},}
$$

where the [Kantorovich potentials](../../../../../../kantorovich-potential.md) are measurable representatives satisfying

$$
\mathcal A_c=\{(u,v):u\in L^1(\mu),\ v\in L^1(\nu),\ u(x)+v(y)\leq c(x,y)\ \text{for every }(x,y)\in X\times Y\}.
$$

One standard form of the [Kantorovich duality theorem](../../../../../../kantorovich-duality-theorem.md) assumes that $X,Y$ are [Polish spaces](../../../../../../polish-space.md), $\mu,\nu$ are [probability measures](../../../../../../probability-measure.md) defined as [Borel measures](../../../../../../borel-measure.md), and $c:X\times Y\to[0,+\infty]$ is [sequentially lower semicontinuous](../../../../../../sequential-lower-semicontinuity.md). Then

$$
\boxed{\min_{\pi\in\Pi(\mu,\nu)}\int c\,d\pi
=\sup_{(u,v)\in\mathcal A_c}\left(\int u\,d\mu+\int v\,d\nu\right).}
$$

The primal infimum is attained; its value may be $+\infty$. Nonnegativity can be replaced by a constant lower bound by shifting the cost. This duality for lower semicontinuous costs is also discussed in [Beiglboeck, Leonard and Schachermayer's duality paper](https://arxiv.org/abs/0911.4347).

**Equality of values does not by itself assert a dual maximum.** A sufficient stronger setting for attainment on both sides is [compact metric spaces](../../../../../../compact-metric-space.md) $X,Y$ and a finite [continuous](../../../../../../continuous-function.md) cost $c$; then [continuous](../../../../../../continuous-function.md) [Kantorovich potentials](../../../../../../kantorovich-potential.md) attain the dual supremum. The general statement above correctly uses a supremum.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 348](../../../paper-348-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

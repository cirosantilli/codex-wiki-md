<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [probability space](../../../../../../probability-space.md) $([0,1]^{\mathbb Z^d},\mathcal F,\mathbb P)$ with the [product measure](../../../../../../product-measure.md) of the [uniform distribution](../../../../../../continuous-uniform-distribution.md) on $[0,1]$. Its coordinate [random variables](../../../../../../random-variable-split.md) $U_v$ are [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md). Define simultaneously for every parameter

$$
\boxed{X_p(v)=\mathbf1_{\{U_v\leq p\}},\qquad p\in[0,1],\ v\in\mathbb Z^d}.
$$

For $r\leq s$, the [indicator function](../../../../../../indicator-function.md) inequality $X_r(v)\leq X_s(v)$ holds pointwise at every [graph vertex](../../../../../../vertex-graph-theory.md). For fixed $p$, each coordinate has the [Bernoulli distribution](../../../../../../bernoulli-distribution.md) with parameter $p$, and the coordinates are independent because they are functions of distinct independent $U_v$. Thus every marginal configuration is exactly the required [site percolation](../../../../../../site-percolation-split.md) model. This is a continuum-indexed family of processes, all on one [probability space](../../../../../../probability-space.md), and is the standard [monotone coupling of Bernoulli percolation](../../../../../../monotone-coupling-of-bernoulli-percolation.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 204](../../../paper-204-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

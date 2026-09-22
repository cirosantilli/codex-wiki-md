<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Markov kernel](../../../../../../markov-kernel.md) $K$ with [stationary distribution](../../../../../../stationary-distribution.md) $\pi$ is [geometrically ergodic](../../../../../../geometric-ergodicity.md) if there are $\rho<1$ and a finite function $M(x)$ such that

$$
\lVert K^m(x,\mathord\cdot)-\pi\rVert_{\mathrm{TV}}
\leq M(x)\rho^m
$$

for every $m\geq0$ and almost every starting point $x$, where $\lVert\cdot\rVert_{\mathrm{TV}}$ is [total variation distance](../../../../../../total-variation-distance.md).

A measurable set $A$ is a [small set](../../../../../../small-set.md) with minorisation constant $\alpha>0$ if some integer $r\geq1$ and some [probability measure](../../../../../../probability-measure.md) $\nu$ satisfy

$$
K^r(x,B)\geq\alpha\nu(B)
$$

for every $x\in A$ and every measurable $B$.

A standard [drift-minorisation condition](../../../../../../drift-minorisation-condition.md) is that the chain be [irreducible](../../../../../../irreducible-markov-chain.md) and [aperiodic](../../../../../../aperiodic-markov-chain.md), and that there exist a measurable $V\geq1$, a small set $A$, constants $\lambda<1$ and $b<\infty$ such that

$$
KV(x)\leq\lambda V(x)+b\mathbf1_A(x).
$$

These conditions imply geometric ergodicity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

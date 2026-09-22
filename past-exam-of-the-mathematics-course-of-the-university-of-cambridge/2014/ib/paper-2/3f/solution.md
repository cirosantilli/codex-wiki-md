<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

A function $f:E\to\mathbb R$ has [uniform continuity](../../../../../uniform-continuity.md) if for every $\varepsilon>0$ there is a $\delta>0$ such that, for all $x,y\in E$, $|x-y|<\delta$ implies $|f(x)-f(y)|<\varepsilon$. The same $\delta$ must work everywhere in $E$.

**The product need not be uniformly continuous.** Both $f(x)=x$ and $g(x)=x$ are [Lipschitz continuous](../../../../../lipschitz-continuity.md), hence uniformly continuous on $\mathbb R$, but their product is $x^2$. For $x_n=n$ and $y_n=n+1/n$, the input separation tends to zero while

$$
|y_n^2-x_n^2|=2+\frac1{n^2}\ge2.
$$

This contradicts [uniform continuity](../../../../../uniform-continuity.md). The issue is captured by [products of unbounded uniformly continuous functions](../../../../../products-of-unbounded-uniformly-continuous-functions.md); bounded factors would give a uniform product estimate.

**A uniformly continuous function on $(0,1)$ is bounded.** Take $\delta$ for output tolerance one and cover $(0,1)$ by finitely many intervals of radius less than $\delta$, centred at points $c_1,\ldots,c_m$ in $(0,1)$. Every $x$ is within $\delta$ of some $c_j$, so $|f(x)|\le1+\max_j|f(c_j)|$. This proves the general principle that a [uniformly continuous function on a totally bounded set is bounded](../../../../../uniformly-continuous-function-on-a-totally-bounded-set-is-bounded.md).

**The reciprocal-cosine function is not uniformly continuous.** Take

$$
x_n=\frac1{2\pi n},\qquad y_n=\frac1{(2n+1)\pi}.
$$

Both sequences lie in $(0,1)$, $|x_n-y_n|\to0$, but the two function values are $1$ and $-1$. Their difference is always two, violating the [sequential criterion for uniform continuity](../../../../../sequential-criterion-for-uniform-continuity.md).

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

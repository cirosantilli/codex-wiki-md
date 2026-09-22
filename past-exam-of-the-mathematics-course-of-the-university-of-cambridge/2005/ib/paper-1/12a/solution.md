<h1 id="12a/solution">Solution</h1>

↑ **Parent:** [12A](../12a.md)

The sum of the two [metrics](../../../../../metric.md) is nonnegative and symmetric. It vanishes exactly when both coordinate distances vanish, hence exactly when the two points agree. Adding the two component [triangle inequalities](../../../../../triangle-inequality.md) gives the [triangle inequality](../../../../../triangle-inequality.md) on the [Cartesian product](../../../../../cartesian-product.md), so the displayed function is a [metric](../../../../../metric.md). Moreover,

$$
d_Y(\pi(x_1,y_1),\pi(x_2,y_2))\le d((x_1,y_1),(x_2,y_2)),
$$

so the [projection map](../../../../../projection-map.md) is $1$-[Lipschitz](../../../../../lipschitz-continuity.md) and therefore [continuous](../../../../../continuous-function.md).

To prove [sequential compactness](../../../../../sequentially-compact-space.md) directly from [compactness](../../../../../compact-space.md), take a sequence $(x_n)$ in $X$. If every point $x$ had a neighborhood containing sequence terms at only finitely many indices, these neighborhoods would form an open cover with a finite subcover, implying that only finitely many sequence terms exist, a contradiction. Thus some $x\in X$ has infinitely many indices in every neighborhood. Choose increasing indices $n_k$ with $d_X(x_{n_k},x)<1/k$; then $x_{n_k}\to x\in X$.

Now let $F\subset X\times Y$ be [closed](../../../../../closed-set.md) and suppose $y_n\in\pi(F)$ converges to $y$. Choose $x_n$ such that $(x_n,y_n)\in F$. A [convergent subsequence](../../../../../convergent-subsequence.md) $x_{n_k}\to x$ exists by the preceding argument. In the product [metric](../../../../../metric.md), $(x_{n_k},y_{n_k})\to(x,y)$, and the fact that $F$ is [closed](../../../../../closed-set.md) gives $(x,y)\in F$. Thus $y\in\pi(F)$, proving that the [projection with a compact factor is closed](../../../../../projection-with-a-compact-factor-is-closed.md). The sequential criterion for a [closed set](../../../../../closed-set.md) in a [metric space](../../../../../metric-space.md) follows by choosing points at distance less than $1/k$ from any point of its closure.

For a counterexample without a compact factor, take $X=Y=\mathbb R$ with their usual [metrics](../../../../../metric.md) and

$$
F=\{(x,y):xy=1\}.
$$

The continuous product function makes $F$ [closed](../../../../../closed-set.md), but $\pi(F)=\mathbb R\setminus\{0\}$ is not [closed](../../../../../closed-set.md). Thus **compactness of the discarded factor is essential to the general conclusion**.

## ↑ Ancestors (10)

1. [12A](../12a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

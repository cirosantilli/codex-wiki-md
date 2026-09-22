<h1 id="2g/solution">Solution</h1>

↑ **Parent:** [2G](../2g.md)

Suppose first that $X$ is connected and $f:X\to\mathbb Z$ is continuous. Its image is connected by the [continuous image of a connected space](../../../../../continuous-image-of-a-connected-space.md), but $\mathbb Z$ is discrete, so its only connected nonempty subsets are singletons. Hence $f$ is constant.

Conversely, if $X=U\cup V$ is a disconnection into nonempty disjoint [open sets](../../../../../open-set.md), the [function](../../../../../function-split.md) equal to zero on $U$ and one on $V$ is continuous and nonconstant. This proves the [integer-valued function criterion for connectedness](../../../../../integer-valued-function-criterion-for-connectedness.md).

Now let $f:X\to\mathbb Z$ be continuous under the hypotheses on the family $\mathcal A$. Each restriction $f|_A$ is constant because $A$ is connected. If $A,B\in\mathcal A$, a point of $A\cap B$ shows that their two constants agree. Since the sets cover $X$, $f$ is constant on $X$, and the criterion proves that $X$ is connected. This is the [pairwise-intersecting connected cover](../../../../../pairwise-intersecting-connected-cover.md) argument.

Finally, fix $y_0\in Y$. For each $x\in X$, the set

$$
A_x=(X\times\{y_0\})\cup(\{x\}\times Y)
$$

is connected: its two connected pieces meet at $(x,y_0)$. The sets $A_x$ cover $X\times Y$ and any two share $X\times\{y_0\}$. The preceding result proves that $X\times Y$ is connected, giving the [product of connected spaces](../../../../../product-of-connected-spaces.md) result.

## ↑ Ancestors (10)

1. [2G](../2g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

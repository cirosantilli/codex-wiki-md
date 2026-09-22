<h1 id="22i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A family $\mathcal S\subseteq C(K)$ is [equicontinuous](../../../../../../equicontinuity.md) if for every $x\in K$ and $\varepsilon>0$ there is a [neighborhood](../../../../../../neighbourhood-mathematics.md) $U$ of $x$ such that

$$
|f(y)-f(x)|<\varepsilon
$$

for every $y\in U$ and every $f\in\mathcal S$. The [Arzelà-Ascoli theorem](../../../../../../arzela-ascoli-theorem.md) says that, for a [compact Hausdorff space](../../../../../../compact-hausdorff-space.md) $K$, a subset of $C(K)$ has [compact closure](../../../../../../relatively-compact-subset.md) in the [uniform norm](../../../../../../supremum-norm.md) if and only if it is equicontinuous and pointwise bounded. On compact $K$, equicontinuity and pointwise boundedness together imply [uniform boundedness](../../../../../../uniformly-bounded-family-of-functions.md).

For necessity, a compact closure is [totally bounded](../../../../../../totally-bounded-space.md). Given $\varepsilon>0$, choose a finite $\varepsilon/3$-net $f_1,\ldots,f_m$. The finitely many [continuous functions](../../../../../../continuous-function.md) $f_j$ are simultaneously continuous near each point, and comparison with a nearby $f_j$ proves equicontinuity of the whole family. Evaluation at any fixed point is a continuous map $C(K)\to\mathbb R$ or $\mathbb C$, so compactness also gives pointwise boundedness.

Conversely, equicontinuity gives, around each $x\in K$, a neighborhood on which every $f\in\mathcal S$ oscillates by less than $\varepsilon/3$. [Compactness](../../../../../../compact-space.md) supplies a finite such cover with selected points $x_1,\ldots,x_m$. Pointwise boundedness makes the set of vectors

$$
\{(f(x_1),\ldots,f(x_m)):f\in\mathcal S\}
$$

a bounded subset of a finite-dimensional [normed vector space](../../../../../../normed-vector-space.md), so it has a finite $\varepsilon/3$-net. Choose one function of $\mathcal S$ for every nonempty cell of this net. If two functions have evaluation vectors in the same cell, then comparison at a selected $x_j$ and the two oscillation bounds show that their uniform distance is less than $\varepsilon$. Thus $\mathcal S$ is totally bounded. Since $C(K)$ is a [Banach space](../../../../../../banach-space-split.md), its closure is complete; a [complete totally bounded metric space is compact](../../../../../../complete-totally-bounded-metric-space-is-compact.md), proving the theorem.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [22I](../../22i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

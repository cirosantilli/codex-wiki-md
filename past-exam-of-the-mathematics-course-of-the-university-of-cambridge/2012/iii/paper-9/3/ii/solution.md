<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The function $x e^{-x}$ is strictly increasing on $(0,1)$ and strictly decreasing on $(1,\infty)$. Hence for each $\lambda>1$ there is a unique $\theta=\lambda^*\in(0,1)$ with $\theta e^{-\theta}=\lambda e^{-\lambda}$.

Apply the subcritical component estimates to $G(n,\theta/n)$. For a specified [vertex](../../../../../../vertex-graph-theory.md), the exact [tree-component expectation in the Erdős-Rényi model](../../../../../../tree-component-expectation-in-the-erdos-renyi-model.md) gives the limiting [probability](../../../../../../probability.md) that it lies in a [tree component](../../../../../../tree-component.md) of order $j$:

$$
a_j=\frac{j^{j-1}}{j!}\theta^{j-1}e^{-\theta j}.
$$

For each fixed $j$, the [probability](../../../../../../probability.md) of a non-tree [graph component](../../../../../../component-graph-theory.md) of that size is $O_j(1/n)$: a [spanning tree](../../../../../../spanning-tree.md) and one extra [edge](../../../../../../edge-of-a-graph.md) are necessary. Moreover the [Galton-Watson process](../../../../../../galton-watson-process.md) exploration estimate from the preceding proof bounds the [probability](../../../../../../probability.md) of order greater than $K$ by $e^{-\delta_\theta(K-1)}$, uniformly in $n$, where $\delta_\theta=\theta-1-\log\theta>0$. First let $n\to\infty$ for fixed $K$, then let $K\to\infty$. No [probability](../../../../../../probability.md) mass escapes to large components or non-tree components, so $\sum_{j\geq1}a_j=1$. Multiplying by $\theta$ and using its defining identity gives

$$
\boxed{\sum_{j=1}^\infty\frac{j^{j-1}}{j!}(\lambda e^{-\lambda})^j=\lambda^*.}
$$

Equivalently, the [rooted-tree generating function](../../../../../../rooted-tree-generating-function.md) selects the smaller solution of $T e^{-T}=\lambda e^{-\lambda}$. The choice of that branch is essential; the larger solution $\lambda$ is not the value of this convergent series.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

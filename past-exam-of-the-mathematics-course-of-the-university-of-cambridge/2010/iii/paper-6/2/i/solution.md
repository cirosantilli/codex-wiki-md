<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**False.** We construct a [compact Hausdorff space](../../../../../../compact-hausdorff-space.md) with a countable dense discrete subspace but no compatible [metric](../../../../../../metric.md). Let

$$
P=\{0,1\}^{\mathcal P(\mathbb N)},\qquad
j(n)_S=\begin{cases}1&n\in S,\\0&n\notin S,\end{cases}
$$

for each subset $S\subseteq\mathbb N$. Give $P$ its [product topology](../../../../../../product-topology.md), and let $X=\overline{j(\mathbb N)}$ in $P$. The [Tychonoff theorem](../../../../../../tychonoff-s-theorem.md) makes $P$ compact, and the product is Hausdorff; hence $X$ is a [compact Hausdorff space](../../../../../../compact-hausdorff-space.md). By construction, $Y=j(\mathbb N)$ is countable and dense in $X$, so $X$ is a [separable topological space](../../../../../../separable-topological-space.md). The coordinate $S=\{n\}$ isolates $j(n)$ within $Y$. Thus the subspace topology on $Y$ is discrete and is induced by the [discrete metric](../../../../../../discrete-metric.md).

Suppose $X$ were metrizable. An infinite sequence of distinct points of $Y$ would have a convergent subsequence, by sequential compactness of a [compact metric space](../../../../../../compact-metric-space.md). Write this subsequence as $j(n_k)$ with distinct $n_k$. For $S=\{n_2,n_4,n_6,\ldots\}$, its $S$ coordinate alternates between zero and one and therefore does not converge. But coordinate projections are continuous in the [product topology](../../../../../../product-topology.md), so every coordinate of a convergent sequence must converge. This contradiction proves that $X$ is not metrizable. This is a [separable compactification need not be metrizable](../../../../../../separable-compactification-need-not-be-metrizable.md) counterexample.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

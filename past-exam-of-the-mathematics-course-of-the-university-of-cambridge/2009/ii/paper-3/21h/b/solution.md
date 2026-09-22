<h1 id="21h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume first that $\overline{\mathcal F}$ is compact in the [supremum norm](../../../../../../supremum-norm.md). A finite norm-net shows that the norms of its members are bounded, so pointwise boundedness follows. Given $x$ and $\varepsilon>0$, choose a finite $\varepsilon/3$-net $g_1,\ldots,g_N$ in the closure. Their continuity gives a common neighborhood $U$ of $x$ where $|g_j(y)-g_j(x)|<\varepsilon/3$ for every $j$. For any $f\in\mathcal F$, choose $g_j$ with $\|f-g_j\|_\infty<\varepsilon/3$; the [triangle inequality](../../../../../../triangle-inequality.md) then gives $|f(y)-f(x)|<\varepsilon$. Thus the family is equicontinuous.

Conversely, suppose pointwise boundedness and equicontinuity. For a prescribed $\varepsilon>0$, choose neighborhoods $U_x$ where every $f$ varies from $f(x)$ by less than $\varepsilon/3$. Compactness supplies a finite subcover $U_{x_1},\ldots,U_{x_N}$. Pointwise boundedness makes the set of vectors $(f(x_1),\ldots,f(x_N))$ bounded in $\mathbb R^N$. Partition a bounding box into finitely many boxes of coordinate diameter less than $\varepsilon/3$, and choose one function from each occupied box. If $f,g$ belong to the same box and $y\in U_{x_j}$, then

$$
|f(y)-g(y)|\le |f(y)-f(x_j)|+|f(x_j)-g(x_j)|+|g(x_j)-g(y)|<\varepsilon.
$$

The chosen functions are therefore a finite $\varepsilon$-net in the [supremum norm](../../../../../../supremum-norm.md). Thus $\mathcal F$ is totally bounded. Its closure is complete and totally bounded, hence compact. To recall the last metric-space fact, successively selecting subsequences in balls of radii $2^{-j}$ produces a Cauchy diagonal subsequence from every sequence; completeness supplies its limit. This proves both directions of the [Arzelà-Ascoli theorem](../../../../../../arzela-ascoli-theorem.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [21H](../../21h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="6/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $v_1\ldots v_k$ be a longest [path](../../../../../continuous-path.md) in the finite simple [graph](../../../../../graph-split.md). Every neighbor of either endpoint lies on this path, since an outside neighbor would extend it. Define two subsets of $\{1,\ldots,k-1\}$:

$$
I=\{i:v_1v_{i+1}\in E\},\qquad J=\{i:v_iv_k\in E\}.
$$

Their sizes are $d(v_1)$ and $d(v_k)$. The degree hypothesis gives $|I|+|J|\geq n\geq k$, but there are only $k-1$ possible indices. Hence some $i$ belongs to both. The edges at that index close a cycle through every vertex of the path:

$$
v_1,v_2,\ldots,v_i,v_k,v_{k-1},\ldots,v_{i+1},v_1.
$$

The [graph](../../../../../graph-split.md) is connected: any component has at least $n/2+1$ vertices by the minimum degree, so two components would exceed $n$ vertices. If $k<n$, connectedness gives an edge from this cycle to an outside vertex. Starting at that vertex and traversing the cycle without its closing edge gives a path with $k+1$ vertices, a contradiction.

Thus $k=n$ and the cycle is a [Hamilton cycle](../../../../../hamilton-cycle.md), proving **[Dirac's theorem](../../../../../dirac-s-theorem.md)**. The overlap-of-indices argument is why the degree threshold is half the number of vertices.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

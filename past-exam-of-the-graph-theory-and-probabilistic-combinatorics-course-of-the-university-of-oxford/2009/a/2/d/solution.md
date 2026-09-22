<h1 id="a/2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the [complete graph](../../../../../complete-graph.md), $p_{K_n}(x)=x(x-1)\cdots(x-n+1)>0$ whenever $x>n-1$.

Use [induction](../../../../../mathematical-induction.md) on the number of vertices, and for fixed $n$ on the number of missing edges. If $G$ is not complete, choose a missing edge $e$ and put $H=G+e$. The recurrence rearranges as

$$
p_G(x)=p_H(x)+p_{H/e}(x).
$$

The first term is positive by the missing-edge [induction](../../../../../mathematical-induction.md). The second [graph](../../../../../graph-split.md) has $n-1$ vertices, so the vertex [induction](../../../../../mathematical-induction.md) makes its [polynomial](../../../../../polynomial-split.md) positive for $x>n-2$, in particular for the present range. The one-vertex base case is $x>0$. Thus **$p_G(x)>0$ for all $x>n-1$**, including noninteger $x$; counting colorings alone would not establish that real-variable claim.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

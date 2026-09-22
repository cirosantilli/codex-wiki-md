<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $a=kn/(2k+1)$, $u=(k+1)n/(2k+1)$ and $b=u/k$. A [graph cut](../../../../../../graph-cut.md) with no crossing [edges](../../../../../../edge-of-a-graph.md) is obtained by assigning whole [graph components](../../../../../../component-graph-theory.md) to its two sides. Among all such assignments, maximize the smaller side's size $S\leq n/2$, and write $T=n-S$ for the other side.

Suppose $S<a$. Then $T>u=kb$. If a [graph component](../../../../../../component-graph-theory.md) on the larger side had size $0<w<n-2S$, moving it to the smaller side would make both $S+w$ and $T-w$ greater than $S$. That contradicts maximality. Hence every [graph component](../../../../../../component-graph-theory.md) on the larger side has at least $n-2S$ [vertices](../../../../../../vertex-graph-theory.md). Since each has at most $b$ [vertices](../../../../../../vertex-graph-theory.md) and their total exceeds $kb$, there must be at least $k+1$ of them. Consequently

$$
n-S=T\geq(k+1)(n-2S),\qquad S\geq\frac{kn}{2k+1}=a,
$$

a contradiction. Thus $a\leq S\leq T\leq u$, proving the **required empty cut with both sides at most $(k+1)n/(2k+1)$**. This [balanced component cut](../../../../../../balanced-component-cut.md) argument works for arbitrary positive component weights as well; it does not require divisibility of $n$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Start with zero [flow](../../../../../../flow.md) and apply the [Ford-Fulkerson algorithm](../../../../../../ford-fulkerson-algorithm.md). The following [augmenting paths](../../../../../../augmenting-path.md) and bottlenecks use the capacities in the original PDF diagram:

$$
\begin{array}{c|l|c|c}
\text{step}&\text{path}&\text{increment}&\text{total flow}\\\hline
1&1\to2\to4\to6\to8&2&2\\
2&1\to2\to5\to6\to8&2&4\\
3&1\to3\to5\to7\to8&1&5\\
4&1\to3\to5\to4\to6\to7\to8&1&6
\end{array}.
$$

For example, the second path is limited by the remaining capacity two on $6\to8$ and by capacity two on $5\to6$. After the third augmentation, $7\to8$ has residual capacity one; the fourth path supplies it through $5\to4\to6\to7$. Every displayed increment is the smallest residual capacity of its path.

The resulting arc flows are

$$
\begin{array}{c|rrrrrrrrrrrrr}
\text{arc}&12&13&23&24&25&35&54&46&56&57&67&68&78\\\hline
f&4&2&0&2&2&2&1&3&2&1&1&4&2
\end{array}.
$$

Here $uv$ denotes $u\to v$. These satisfy every capacity bound and [flow conservation](../../../../../../flow-conservation.md). The final [residual network](../../../../../../residual-network.md) has source-reachable set $S=\{1,2,3,5\}$. Its outgoing arcs are $2\to4$, $5\to4$, $5\to6$ and $5\to7$, with capacities $2,1,2,1$, all saturated. Consequently

$$
\boxed{|f|_{\max}=6,\qquad (S,S^c)=(\{1,2,3,5\},\{4,6,7,8\}),\qquad c(S,S^c)=6.}
$$

This is a [minimum cut](../../../../../../minimum-cut.md), and the equal flow and cut values certify optimality by the [max-flow min-cut theorem](../../../../../../max-flow-min-cut-theorem.md). The cut immediately before node eight also has capacity six, so the minimum cut is not unique.

<a id="3/b/image-maximum-flow-six-and-a-minimum-cut-with-arc-labels-showing-flow-capacity"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-35-maximum-flow.png)

**[Figure 1](#3/b/image-maximum-flow-six-and-a-minimum-cut-with-arc-labels-showing-flow-capacity). Maximum flow six and a minimum cut, with arc labels showing flow/capacity**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

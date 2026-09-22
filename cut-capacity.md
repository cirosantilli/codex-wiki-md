# Cut capacity

↑ **Parent:** [Cut of a flow network](cut-of-a-flow-network.md)

The [cut capacity](cut-capacity.md) of $(S,S^c)$, with $S^c=V\setminus S$ the [complement of a set](complement-of-a-set.md), is

$$
c(S,S^c)=\sum_{(u,v)\in E:\,u\in S,\,v\notin S}c_{uv}.
$$

Only outward [directed edges](directed-edge.md) contribute; incoming and internal [edges](edge-of-a-graph.md) contribute nothing.[Algorithms, 4th edition by Robert Sedgewick and others; Sedgewick and Wayne, FordFulkerson.java, check method, lines 196–203: sum capacities only from the source side to its complement](algorithms-4th-edition-by-robert-sedgewick-and-others/fordfulkerson-java.md)

Here is the accounting behind the bound, using nonnegative original [edge](edge-of-a-graph.md) amounts $f_{uv}$ in a finite [flow network](flow-network-split.md). Sum the [divergence of a flow](divergence-of-a-flow.md) over the [vertices](vertex-graph-theory.md) in $S$:

$$
\sum_{v\in S}\operatorname{div}f(v)
=\sum_{v\in S}\left(\sum_{w:(v,w)\in E}f_{vw}-\sum_{u:(u,v)\in E}f_{uv}\right).
$$

An [edge](edge-of-a-graph.md) with both endpoints in $S$ appears once with a plus sign at its tail and once with a minus sign at its head, so those contributions cancel. An outward [edge](edge-of-a-graph.md) appears only with a plus sign; an incoming [edge](edge-of-a-graph.md) appears only with a minus sign. Since $s\in S$, $t\notin S$ and every other [vertex](vertex-graph-theory.md) satisfies [flow conservation](flow-conservation.md), the left side is the [flow value](strength-of-a-flow.md). Thus

$$
|f|=\sum_{(u,v)\in E:\,u\in S,\,v\notin S}f_{uv}
-\sum_{(u,v)\in E:\,u\notin S,\,v\in S}f_{uv}
\leq\sum_{(u,v)\in E:\,u\in S,\,v\notin S}c_{uv}=c(S,S^c).
$$

The inequality uses two facts separately: each forward [flow](flow.md) is at most its [flow network edge capacity](flow-network-edge-capacity.md), and each backward [flow](flow.md) is nonnegative. This is the [weak duality](weak-duality.md) bound underlying the [max-flow min-cut theorem](max-flow-min-cut-theorem.md). It is an accounting proof, requiring no choice of [augmenting paths](augmenting-path.md).

For $S=\{s,b\}$ in the running example, explicitly add the two [divergences of a flow](divergence-of-a-flow.md):

$$
\operatorname{div}f(s)+\operatorname{div}f(b)
=(f_{sa}+f_{sb})+(f_{bt}-f_{sb}-f_{ab})
=f_{sa}+f_{bt}-f_{ab}=3+3-1=5.
$$

The internal $s\to b$ [edge](edge-of-a-graph.md) cancels. The $a\to b$ [edge](edge-of-a-graph.md) is a genuine original [directed edge](directed-edge.md) entering $S$, so its [flow](flow.md) is subtracted; this is different from a backward [edge](edge-of-a-graph.md) in a [residual network](residual-network.md). Its [flow network edge capacity](flow-network-edge-capacity.md) is neither added to nor subtracted from [cut capacity](cut-capacity.md), which remains $c_{sa}+c_{bt}=6$.

Equality in the bound holds precisely when every outward [edge](edge-of-a-graph.md) is saturated and every incoming [edge](edge-of-a-graph.md) carries zero [flow](flow.md), because

$$
c(S,S^c)-|f|
=\sum_{(u,v)\in E:\,u\in S,\,v\notin S}(c_{uv}-f_{uv})
+\sum_{(u,v)\in E:\,u\notin S,\,v\in S}f_{uv},
$$

and every term is nonnegative. For $S=\{s\}$ the two outward [edges](edge-of-a-graph.md) are saturated and there are no incoming [edges](edge-of-a-graph.md), so the gap is zero. For $S=\{s,b\}$ all outward [edges](edge-of-a-graph.md) are still saturated, but the incoming [flow](flow.md) of $1$ gives a gap of $1$. This explains exactly why the second [cut of a flow network](cut-of-a-flow-network.md) is not a [minimum cut](minimum-cut.md).

## ↑ Ancestors (7)

1. [Cut of a flow network](cut-of-a-flow-network.md)
2. [Flow network](flow-network-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Cut capacity](cut-capacity.md)
- [Cut of a flow network](cut-of-a-flow-network.md)
- [Max-flow min-cut theorem](max-flow-min-cut-theorem.md)
- [Maximum flow problem](maximum-flow-problem.md)
- [Minimum cut](minimum-cut.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-4/5h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-4/10g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-33/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-2/9c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-35/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-2/9h/solution.md)
- [Residual network](residual-network.md)
- [Residual reachability certificate for maximum flow](residual-reachability-certificate-for-maximum-flow.md)

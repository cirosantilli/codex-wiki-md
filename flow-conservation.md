# Flow conservation

↑ **Parent:** [Divergence of a flow](divergence-of-a-flow.md)

[Flow conservation](flow-conservation.md) requires equal total inflow and outflow at every [vertex](vertex-graph-theory.md) other than the source and sink:

$$
\sum_{u:(u,v)\in E}f_{uv}=\sum_{w:(v,w)\in E}f_{vw}
\quad(v\notin\{s,t\}).
$$

Equivalently, the [divergence of a flow](divergence-of-a-flow.md) is zero there.[Algorithms, 4th edition by Robert Sedgewick and others; Sedgewick and Wayne, FordFulkerson.java, excess and isFeasible methods, lines 138–175: incoming minus outgoing amount and zero excess at nonterminal vertices](algorithms-4th-edition-by-robert-sedgewick-and-others/fordfulkerson-java.md)

This is a steady accounting condition: an intermediate [vertex](vertex-graph-theory.md) neither creates the routed resource nor accumulates it. Splitting is allowed; equality between individual incoming and outgoing [edges](edge-of-a-graph.md) is not required. For the running [flow](flow.md), the equation at $a$ is $f_{sa}=f_{ab}+f_{at}$, or $3=1+2$, and at $b$ it is $f_{sb}+f_{ab}=f_{bt}$, or $2+1=3$.

[Capacity constraints](capacity-constraint.md) alone do not ensure [flow conservation](flow-conservation.md). For instance, changing only $f_{ab}$ from $1$ to $0$ keeps every [edge](edge-of-a-graph.md) amount within its [flow network edge capacity](flow-network-edge-capacity.md), but leaves an excess inflow of $1$ at $a$ and an excess outflow of $1$ at $b$. It is therefore not a [feasible flow](feasible-flow.md). Changing all affected [edge](edge-of-a-graph.md) amounts together to $(f_{sa},f_{sb},f_{ab},f_{at},f_{bt})=(2,2,0,2,2)$ restores both equations and gives [flow value](strength-of-a-flow.md) $4$.

## ↑ Ancestors (8)

1. [Divergence of a flow](divergence-of-a-flow.md)
2. [Flow](flow.md)
3. [Flow network](flow-network-split.md)
4. [Graph theory](graph-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (33)

- [Augmenting path](augmenting-path.md)
- [Cut capacity](cut-capacity.md)
- [Divergence of a flow](divergence-of-a-flow.md)
- [Flow](flow.md)
- [Flow balance](flow-balance.md)
- [Flow conservation](flow-conservation.md)
- [Flow network](flow-network-split.md)
- [Fundamental cycle](fundamental-cycle.md)
- [Kirchhoff node law](kirchhoff-node-law.md)
- [Max-flow min-cut theorem](max-flow-min-cut-theorem.md)
- [Maximum flow problem](maximum-flow-problem.md)
- [Minimum cut](minimum-cut.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-4/5h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-4/10g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-33/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-2/9c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-38/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-1/8c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2/8d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2/9h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-35/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-35/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4/20h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/20h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/20h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/20h/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-214/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/20h/a/solution.md)
- [Residual network](residual-network.md)
- [Residual reachability certificate for maximum flow](residual-reachability-certificate-for-maximum-flow.md)
- [Strength of a flow](strength-of-a-flow.md)
- [Treatment capacity as a sink arc](treatment-capacity-as-a-sink-arc.md)
- [Vertex capacity](vertex-capacity.md)

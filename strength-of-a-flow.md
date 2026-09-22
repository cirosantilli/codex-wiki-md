# Strength of a flow

↑ **Parent:** [Flow](flow.md)

The [strength of a flow](strength-of-a-flow.md), also called its [flow value](strength-of-a-flow.md), is net outflow from $s$, equivalently net inflow to $t$:

$$
|f|=\sum_{v:(s,v)\in E}f_{sv}-\sum_{u:(u,s)\in E}f_{us}
=\sum_{u:(u,t)\in E}f_{ut}-\sum_{v:(t,v)\in E}f_{tv}.
$$

The notation $|f|$ denotes this signed value, rather than an absolute value.[Graph Theory by Reinhard Diestel; Diestel, Flows, §6.2, printed p. 159: total value after Proposition 6.2.1 and footnote 4 on possible negative values](graph-theory-by-reinhard-diestel/flows-author-hosted-chapter-preview.md)

The equality follows by summing the [divergence of a flow](divergence-of-a-flow.md) over all [vertices](vertex-graph-theory.md): the internal [vertices](vertex-graph-theory.md) contribute zero by [flow conservation](flow-conservation.md), while every [edge](edge-of-a-graph.md) cancels between its two endpoints. Hence $\operatorname{div}f(s)=-\operatorname{div}f(t)$. For the running [flow](flow.md), $|f|=3+2=2+3=5$.

Net outflow matters even when the source has incoming [edges](edge-of-a-graph.md). As a separate example, give $s\to a$, $a\to s$ and $s\to t$ [flow network edge capacities](flow-network-edge-capacity.md) $2,2,3$ and [flow](flow.md) amounts $2,2,3$. At $a$, [flow conservation](flow-conservation.md) reads $2=2$. The source sends $5$ units along outgoing [edges](edge-of-a-graph.md) but receives $2$ back, so the [flow value](strength-of-a-flow.md) is $5-2=3$, exactly the amount arriving at $t$. The two-[edge](edge-of-a-graph.md) [network circulation](circulation-in-a-flow-network.md) through $a$ raises total [edge](edge-of-a-graph.md) usage without increasing net delivery.

## ↑ Ancestors (7)

1. [Flow](flow.md)
2. [Flow network](flow-network-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Augmenting path](augmenting-path.md)
- [Max-flow min-cut theorem](max-flow-min-cut-theorem.md)
- [Maximum flow problem](maximum-flow-problem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-35/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/20h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/20h/b/solution.md)
- [Residual reachability certificate for maximum flow](residual-reachability-certificate-for-maximum-flow.md)
- [Strength of a flow](strength-of-a-flow.md)
- [Unit flow](unit-flow.md)

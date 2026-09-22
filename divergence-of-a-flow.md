# Divergence of a flow

↑ **Parent:** [Flow](flow.md)

The [divergence of a flow](divergence-of-a-flow.md) at a [vertex](vertex-graph-theory.md) $v$ is net outward [flow](flow.md). For original nonnegative [edge](edge-of-a-graph.md) amounts and their signed net record, respectively,

$$
\operatorname{div}f(v)
=\sum_{w:(v,w)\in E}f_{vw}-\sum_{u:(u,v)\in E}f_{uv}
=\sum_{w\in V}\theta_{vw}.
$$

Positive [divergence of a flow](divergence-of-a-flow.md) means net supply, negative [divergence of a flow](divergence-of-a-flow.md) means net demand, and zero is [flow conservation](flow-conservation.md). This is the same sign convention as [flow balance](flow-balance.md).

In the running example, the [divergences of a flow](divergence-of-a-flow.md) at $(s,a,b,t)$ are $(5,0,0,-5)$. Adding the four [divergences of a flow](divergence-of-a-flow.md) gives zero: every [edge](edge-of-a-graph.md) contributes positively at one endpoint and negatively at the other. In a finite [flow network](flow-network-split.md), this cancellation explains why net supply at $s$ equals net demand at $t$.

**Table of contents**

- [Flow conservation](flow-conservation.md)

## ↑ Ancestors (7)

1. [Flow](flow.md)
2. [Flow network](flow-network-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Cut capacity](cut-capacity.md)
- [Divergence of a flow](divergence-of-a-flow.md)
- [Flow](flow.md)
- [Flow conservation](flow-conservation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-30/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-212/2/a/solution.md)
- [Strength of a flow](strength-of-a-flow.md)
- [Unit flow](unit-flow.md)

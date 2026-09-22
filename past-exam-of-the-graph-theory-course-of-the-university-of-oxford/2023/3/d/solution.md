<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

We verify the [Hall condition](../../../../hall-condition.md) for $U$. Let $S\subseteq U$. If $S$ is empty, then $|N(S)|=0=|S|$. Suppose $0<|S|\leq n/2$. Choose $u\in S$. Its [graph neighbourhood](../../../../graph-neighbourhood.md) is contained in $N(S)$, so the [minimum degree](../../../../minimum-degree-of-a-graph.md) hypothesis gives

$$
|N(S)|\geq d_G(u)\geq n/2\geq|S|.
$$

If $|S|>n/2$, suppose for a contradiction that some [vertex](../../../../vertex-graph-theory.md) $w\in W\setminus N(S)$ exists. All [neighbours](../../../../neighbour-of-a-vertex.md) of $w$ lie in $U\setminus S$, so

$$
d_G(w)\leq n-|S|<n/2,
$$

contradicting the [minimum degree](../../../../minimum-degree-of-a-graph.md) hypothesis. Thus $N(S)=W$ and $|N(S)|=n\geq|S|$.

Every [subset](../../../../subset.md) $S\subseteq U$ satisfies the [Hall condition](../../../../hall-condition.md). By [Hall's marriage theorem](../../../../hall-s-marriage-theorem.md), there is a [matching in a graph](../../../../matching-graph-theory-split.md) saturating $U$. Since $|U|=|W|=n$, its $n$ [edges](../../../../edge-of-a-graph.md) also cover every [vertex](../../../../vertex-graph-theory.md) of $W$. It is therefore a **complete matching**, meaning a [perfect matching](../../../../perfect-matching.md). For $n=0$, the empty [matching in a graph](../../../../matching-graph-theory-split.md) already has this property.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the graph theory course of the University of Oxford](../../../split.md)
5. [Graph theory course of the University of Oxford](../../../../graph-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use a [dynamic programming state](../../../../../dynamic-programming-state.md) indexed by an [edge](../../../../../edge-of-a-graph.md) budget. Put $D_0(s)=0$ and $D_0(v)=\infty$ for $v\ne s$, then for $r=1,\ldots,k$ compute

$$
\boxed{D_r(v)=\min\left(D_{r-1}(v),\ \min_{(u,v)\in E}\{D_{r-1}(u)+w(u,v)\}\right).}
$$

Every route using at most $r$ [edges](../../../../../edge-of-a-graph.md) either already uses at most $r-1$, or ends with some [edge](../../../../../edge-of-a-graph.md) $(u,v)$ whose preceding route uses at most $r-1$. Conversely every finite candidate in the displayed equation is attained by such a route. This proves the [hop-bounded shortest-route recurrence](../../../../../hop-bounded-shortest-route-recurrence.md) by [induction](../../../../../mathematical-induction.md) on $r$, even when weights are negative.

In each round, copy the previous distance row and relax every [edge](../../../../../edge-of-a-graph.md) into the new row, always reading from the old row. An in-place pass would allow several new [edges](../../../../../edge-of-a-graph.md) in one round and violate the [edge](../../../../../edge-of-a-graph.md) budget. Store a predecessor record for every selected candidate, either a carry to $(r-1,v)$ or the incoming [edge](../../../../../edge-of-a-graph.md) from $(r-1,u)$. Following records backwards from $(k,t)$ and reversing the collected [edges](../../../../../edge-of-a-graph.md) returns the actual optimum route; an infinite final distance means no feasible route exists.

Only [vertices](../../../../../vertex-graph-theory.md) incident to an [edge](../../../../../edge-of-a-graph.md), together with $s,t$, need distance fields. In a graph representation whose [edges](../../../../../edge-of-a-graph.md) reference [vertex](../../../../../vertex-graph-theory.md) records, initialise those fields by visiting both endpoints of every [edge](../../../../../edge-of-a-graph.md), then $s,t$; repeated initialisations are harmless. In each round, first copy old fields to new fields by another complete endpoint pass, and only then begin the relaxation pass. Copying the same endpoint several times before any relaxation also does no harm. Thus each round costs $O(m+1)$, with no scan of isolated [vertices](../../../../../vertex-graph-theory.md), and for $m,k\ge1$ the total is **$O(km)$ time**. An implementation that instead initialises full arrays for all [vertices](../../../../../vertex-graph-theory.md) has the conventional bound $O(|V|+km)$. For $k=0$ or no [edges](../../../../../edge-of-a-graph.md), only the empty route $s=t$ can succeed.

To realise reconstruction without a dense table, associate a persistent route record with each finite distance. A successful relaxation in round $r$ creates a record containing the new [edge](../../../../../edge-of-a-graph.md) and a pointer to the old round's route record at its source; a carry shares its record. All reads use old-round records. At most $km$ such records are created, taking $O(km)$ space, and the returned chain has at most $k$ [edges](../../../../../edge-of-a-graph.md). Distances alone need only two fields per relevant [vertex](../../../../../vertex-graph-theory.md).

Here “route” uses the standard edge-budget shortest-path convention permitting repeated [vertices](../../../../../vertex-graph-theory.md); a bounded budget prevents an arbitrarily long negative-cycle traversal. If “path” instead requires [vertex](../../../../../vertex-graph-theory.md) simplicity with unrestricted negative weights, this recurrence does not enforce that extra restriction. With nonnegative weights, removing cycles gives a simple optimum within the same budget.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [7](../../7.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

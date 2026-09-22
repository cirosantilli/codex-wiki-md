<h1 id="17f/solution">Solution</h1>

↑ **Parent:** [17F](../17f.md)

For a finite connected [plane graph](../../../../../plane-graph.md), with $v$ [vertices](../../../../../vertex-graph-theory.md), $e$ [edges](../../../../../edge-of-a-graph.md) and $f$ faces including the unbounded face, [Euler formula for a connected planar graph](../../../../../euler-formula-for-a-connected-planar-graph.md) is

$$
\boxed{v-e+f=2.}
$$

If the [graph](../../../../../graph-split.md) is a [tree](../../../../../tree-graph-theory.md), $e=v-1$ and $f=1$. Otherwise remove an [edge](../../../../../edge-of-a-graph.md) on a cycle. This preserves connectivity and joins the two faces on its sides, so both $e$ and $f$ decrease by one. Repeating reaches a [tree](../../../../../tree-graph-theory.md), preserving $v-e+f$ throughout and proving the formula.

For a simple connected [graph](../../../../../graph-split.md) with $v\geq3$, each face boundary walk has length at least three, with bridges counted twice in the walk; the sum of lengths is $2e$. Hence $3f\leq2e$, which with Euler gives **$e\leq3v-6$**. If it has no [triangles in a graph](../../../../../triangle-in-a-graph.md), no face boundary walk can have length three, and every boundary length is at least four. Thus $4f\leq2e$, giving

$$
\boxed{e\leq2v-4\quad\text{for a triangle-free planar graph with }v\geq3.}
$$

For a disconnected [graph](../../../../../graph-split.md), add noncrossing bridges between its components; this preserves simplicity and creates no triangles, reducing to the connected bound.

Every [triangle-free](../../../../../triangle-free-graph.md) [planar graph](../../../../../planar-graph.md) with at least three [vertices](../../../../../vertex-graph-theory.md) has average degree $2e/v<4$, and therefore a [vertex](../../../../../vertex-graph-theory.md) of degree at most three. Remove one such [vertex](../../../../../vertex-graph-theory.md). Its remaining [graph](../../../../../graph-split.md) is again [triangle-free](../../../../../triangle-free-graph.md) and planar. Induction, with [graphs](../../../../../graph-split.md) on at most two [vertices](../../../../../vertex-graph-theory.md) as the base cases, provides a [graph colouring](../../../../../graph-coloring.md) with four colours of the remainder. At most three colours appear on the removed [vertex](../../../../../vertex-graph-theory.md)'s neighbours, so a fourth colour extends the [graph colouring](../../../../../graph-coloring.md). This proves **four-colourability without using the four-colour theorem**.

## ↑ Ancestors (10)

1. [17F](../17f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

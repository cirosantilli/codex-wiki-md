<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the specified construction as a [polynomial-time many-one reduction](../../../../../../polynomial-time-many-one-reduction.md) from [3-SAT](../../../../../../3-sat.md). There are $2n+3m$ vertices and $n+6m$ edges: one edge per variable pair, three edges per clause [triangle in a graph](../../../../../../triangle-in-a-graph.md), and three occurrence edges per clause. Any [vertex cover](../../../../../../vertex-cover.md) must take at least one vertex from every variable pair and at least two from every clause triangle. Therefore every cover has at least $n+2m$ vertices.

Given a satisfying [Boolean valuation](../../../../../../boolean-valuation.md), include the vertex corresponding to the true [Boolean literal](../../../../../../boolean-literal.md) in each variable pair. In each clause choose a true occurrence and omit its clause vertex, including the other two. Every variable edge and triangle edge is covered. An occurrence edge with an included clause endpoint is covered automatically; the only omitted occurrence vertex is joined to the included true-literal vertex. This is a [vertex cover](../../../../../../vertex-cover.md) with exactly $n+2m$ vertices.

Conversely, a cover of that size must use exactly one vertex in each variable pair and exactly two in each triangle. Declare a variable true precisely when its positive-literal vertex is included. Each clause has one omitted vertex. Its occurrence edge forces the corresponding literal vertex into the cover, so that literal is true. Every clause is therefore satisfied. Thus

$$
\boxed{\text{formula satisfiable}\iff\text{constructed graph has a cover of size }n+2m.}
$$

The construction and target size are polynomial in the input length. Since [3-SAT](../../../../../../3-sat.md) is [NP-complete](../../../../../../np-completeness.md), the decision problem is [NP-hard](../../../../../../np-hardness.md). The usual “at most $k$” version has the same equivalence here because $n+2m$ is an unavoidable lower bound. More generally, a cover with fewer than $k\leq|V|$ vertices can be padded to exactly $k$. Verifying a proposed cover is polynomial, so the usual vertex-cover decision problem is also in [NP](../../../../../../np-complexity.md) and hence [NP-complete](../../../../../../np-completeness.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

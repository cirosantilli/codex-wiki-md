<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [lexicographic embedding of a sumset](../../../../../../lexicographic-embedding-of-a-sumset.md): choose the least tuple $(s_1,\ldots,s_n)\in\prod_iS_i$ representing each distinct sum, and let $B$ be the set of those tuples. Then $|B|=|S|$. If two projections onto $A$ had the same partial sum but different tuples, replacing the larger projected tuple by the smaller one inside its full representative would preserve that full sum and improve its lexicographic order. This is impossible. Thus the summation map is injective on the projection $B_A$, giving $|B_A|\leq|S_A|$.

Replace every integer tuple of $B$ by the closed unit cube centered there. Their interiors are disjoint, and each coordinate projection is a union of unit cubes indexed by $B_A$, so the resulting body has volume $|B|$ and projected volume $|B_A|$. Apply the [box theorem](../../../../../../box-theorem.md) to obtain

$$
\boxed{|S|=\prod_i b_i,\qquad |S_A|\geq|B_A|\geq\prod_{i\in A}b_i.}
$$

The empty-set case uses $S_\varnothing=\{0\}$ and the empty product one.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

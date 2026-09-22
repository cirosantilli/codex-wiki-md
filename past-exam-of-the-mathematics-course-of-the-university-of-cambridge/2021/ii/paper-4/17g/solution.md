<h1 id="17g/solution">Solution</h1>

↑ **Parent:** [17G](../17g.md)

[Hall marriage theorem](../../../../../hall-s-marriage-theorem.md) states that a bipartite graph with parts $A,B$ has a matching saturating $A$ iff $|N(S)|\geq|S|$ for every $S\subseteq A$. Starting with a maximum matching, an unmatched vertex and its alternating reachable set would violate Hall unless an augmenting path exists; flipping along that path increases the matching, proving sufficiency.

Every vertex cover meets each edge of a matching, so $γ\leqβ$. Endpoints of a maximal matching cover every edge, so $β\leq2γ$. A disjoint union of $k$ triangles has $(γ,β)=(k,2k)$. For $T_3(30)$, $γ=15$ and $β=30-10=20$. In bipartite graphs the alternating-path proof constructs a cover of size equal to a maximum matching, giving König theorem.

The chromatic index is the minimum number of matchings partitioning the edges. Label vertices of $K_{2^r}$ by the vector space over $\mathbb F_2$; for each nonzero $a$, pair $x$ with $x+a$. These $2^r-1$ perfect matchings partition all edges, while degree gives the matching lower bound, so $χ\prime=n-1$.

## ↑ Ancestors (10)

1. [17G](../17g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

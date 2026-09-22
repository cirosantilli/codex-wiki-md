<h1 id="b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assign each vertex a color independently and uniformly from the five available residues. Let $A_v$ be the event that none of its neighbours has the successor color. Conditional on the color of $v$, its $r$ neighbours all avoid that color with probability $(4/5)^r$, so $P(A_v)=(4/5)^r$.

The event only uses colors in the closed neighbourhood of $v$. Events based on disjoint such sets are jointly independent. A closed neighbourhood can intersect another only when the two centres are at distance at most two, giving dependency [degree](../../../../../degree-of-a-polynomial.md) at most $r+r(r-1)=r^2$. For sufficiently large $r$,

$$
e(r^2+1)(4/5)^r\le1.
$$

The symmetric local lemma therefore supplies a color assignment with no bad event, proving **every vertex has a neighbour of the successor color**. As defined in the question, this is a five-color assignment; it is not required to be a [proper vertex coloring](../../../../../proper-vertex-coloring.md) of every edge, which would be impossible for some large regular graphs.

The construction generalizes to [cyclic successor colorings of regular graphs](../../../../../cyclic-successor-colorings-of-regular-graphs.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

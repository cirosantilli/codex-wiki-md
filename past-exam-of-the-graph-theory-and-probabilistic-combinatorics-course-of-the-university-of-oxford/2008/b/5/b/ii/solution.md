<h1 id="b/5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Orient each edge independently and uniformly. Fix a $k$-set $A$. An outside vertex beats every member of $A$ with probability $2^{-k}$. For different outside vertices these events depend on disjoint sets of edges, so they are independent. Thus

$$
\mathbb P(A\text{ is undominated})=(1-2^{-k})^{n-k}.
$$

A [union bound](../../../../../../boole-s-inequality.md) over all $\binom nk$ possible sets gives

$$
\mathbb P(\text{some }k\text{-set is undominated})\le\binom nk(1-2^{-k})^{n-k}<1.
$$

The complementary event has positive probability, proving **a [tournament](../../../../../../tournament-graph-theory.md) with the required domination property exists**. This applies in the intended nonvacuous range $n\ge k$; the asymptotic construction below has $n>k$.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [B](../../../../b.md)
5. [2008](../../../../../2008-split.md)
6. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../split.md)
7. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)

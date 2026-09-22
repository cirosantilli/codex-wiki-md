<h1 id="b/6/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Color every edge independently and uniformly with one of $k$ colors. For each unoriented simple four-edge path $P$, let $A_P$ be its repetition event. Its four distinct edges must satisfy two prescribed color equalities, so $\mathbb P(A_P)=k^{-2}$.

Events with edge-disjoint paths depend on disjoint random variables. A fixed edge lies on at most $4\Delta^3$ unoriented four-edge paths: count its four possible positions and two orientations, bound the remaining choices by $\Delta^3$, then divide the oriented path count by two. Thus the union of all paths sharing any of $P$'s four edges has size at most $16\Delta^3$. This union includes $P$ itself, so a dependency [graph](../../../../../../graph-split.md) has $d+1\leq16\Delta^3$.

For $k\geq8\Delta^{3/2}$,

$$
e\,k^{-2}(d+1)\leq\frac{16e\Delta^3}{64\Delta^3}=\frac e4<1.
$$

The symmetric [Lovász local lemma](../../../../../../lovasz-local-lemma.md) yields positive [probability](../../../../../../probability.md) of avoiding every event. Therefore **such an [edge coloring](../../../../../../edge-coloring.md) exists**. If there are no four-edge paths the conclusion is immediate.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [B](../../../../b.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../split.md)
7. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)

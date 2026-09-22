<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Define the directed successor relation by $E(u,v)\iff l(u)=c(v)\lor r(u)=c(v)$. Then the required [predicate](../../../../../predicate.md) is

$$
\boxed{\forall u,v\in T.\quad E(u,v)\Rightarrow v(u)<v(v),}
$$

where $v(u)$ denotes the natural-number information component of node $u$. In the source's indexed notation this is $\forall n_i,n_j\in T,\ (l_i=c_j\lor r_i=c_j)\Rightarrow v_i<v_j$.

This formulation checks both successor links against every node with the corresponding identifier, so it does not silently assume part (d)'s uniqueness condition. It checks existing successors; if every identifier must denote an actual node, add the separate [referential integrity](../../../../../referential-integrity.md) condition $\forall u\in T,\ \exists v,w\in T,\ c(v)=l(u)\land c(w)=r(u)$, or exempt an explicitly designated null identifier. The source specifies no null convention. Indeed a nonempty finite structure with two actual successors at every node cannot have strictly increasing values along all edges: following successors would eventually create a [directed cycle](../../../../../directed-cycle.md). The implication above remains meaningful for leaves represented by absent or null successors.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [5](../../5.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

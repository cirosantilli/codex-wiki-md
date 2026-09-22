<h1 id="17h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Factor the proposed polynomial:

$$
f(t)=t(t-1)^2(t-2).
$$

In particular,

$$
f(2)=0.
$$

By the [two-colourability criterion for bipartite graphs](../../../../../../two-colourability-criterion-for-bipartite-graphs.md), every finite [bipartite graph](../../../../../../bipartite-graph.md) has at least one proper two-colouring, so its chromatic polynomial is positive at $2$. Therefore $f$ cannot be the chromatic polynomial of a bipartite graph.

It is nevertheless a chromatic polynomial. Start with the [complete graph](../../../../../../complete-graph.md) $K_3$, whose vertices may be coloured in

$$
t(t-1)(t-2)
$$

ways, and attach one [leaf](../../../../../../leaf-of-a-graph.md) to any vertex. After the triangle is coloured, the leaf has $t-1$ available colours. The [chromatic polynomial after attaching a leaf](../../../../../../chromatic-polynomial-after-attaching-a-leaf.md) therefore gives

$$
\boxed{P_G(t)=t(t-1)(t-2)(t-1)=f(t).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17H](../../17h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

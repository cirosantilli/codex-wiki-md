<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the identification of two-element subsets of $[n]$ with the [edges](../../../../../../edge-of-a-graph.md) of the [complete graph](../../../../../../complete-graph.md) $K_n$. A colour class in the [Kneser graph](../../../../../../kneser-graph.md) $KG(n,2)$ is an [intersecting two-element set family](../../../../../../intersecting-two-element-set-family.md), so its [edges](../../../../../../edge-of-a-graph.md) must pairwise meet.

Such a class is contained either in a [star graph](../../../../../../star-graph-theory.md) or in a [triangle in a graph](../../../../../../triangle-in-a-graph.md). Indeed, if not all [edges](../../../../../../edge-of-a-graph.md) have a common [vertex](../../../../../../vertex-graph-theory.md), take two meeting [edges](../../../../../../edge-of-a-graph.md) $ab,ac$. An [edge](../../../../../../edge-of-a-graph.md) not containing $a$ must then be $bc$. Any further [edge](../../../../../../edge-of-a-graph.md) meeting all three of $ab,ac,bc$ is one of these three. Classes with at most two [edges](../../../../../../edge-of-a-graph.md) already lie in a [star graph](../../../../../../star-graph-theory.md).

Assume that a [graph colouring](../../../../../../graph-coloring.md) used $c\leq n-3$ colours. Classify $s$ classes as stars and the remaining $t=c-s$ classes as triangles. Delete a chosen centre of each star class, leaving $m\geq n-s\geq t+3$ [vertices](../../../../../../vertex-graph-theory.md). Every [edge](../../../../../../edge-of-a-graph.md) between those remaining [vertices](../../../../../../vertex-graph-theory.md) must belong to a triangle class, of which each covers at most three [edges](../../../../../../edge-of-a-graph.md). Hence

$$
\binom m2\leq3t.
$$

But

$$
\binom{t+3}{2}-3t=\frac{t^2-t+6}{2}>0,
$$

a contradiction. Thus $\chi(KG(n,2))\geq n-2$. For the matching upper bound, assign a two-set the colour of its smaller element if that element is at most $n-3$, and otherwise give it colour $n-2$. The last class comprises the three pairs on the last three elements, an [intersecting family](../../../../../../intersecting-family.md). Consequently **an entirely combinatorial argument gives**

$$
\boxed{\chi(KG(n,2))=n-2\quad(n\geq4).}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

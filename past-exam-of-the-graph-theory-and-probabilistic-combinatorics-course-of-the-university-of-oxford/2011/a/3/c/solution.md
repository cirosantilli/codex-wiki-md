<h1 id="a/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply part (b) to $(X_1,X_2)$ and $(X_1,X_3)$. Fewer than $2\varepsilon|X_1|$ [vertices](../../../../../vertex-graph-theory.md) fail at least one of the degree bounds. For any remaining [vertex](../../../../../vertex-graph-theory.md) $v$, put $N_2=N(v)\cap X_2$ and $N_3=N(v)\cap X_3$. Then

$$
|N_2|\geq\frac d2|X_2|\geq\varepsilon|X_2|,\qquad
|N_3|\geq\frac d2|X_3|\geq\varepsilon|X_3|.
$$

Regularity of $(X_2,X_3)$ gives $d(N_2,N_3)\geq d-\varepsilon\geq d/2$. Every [edge](../../../../../edge-of-a-graph.md) between $N_2$ and $N_3$ makes a distinct [triangle](../../../../../triangle-in-a-graph.md) containing $v$. Hence $v$ belongs to at least

$$
\frac d2|N_2||N_3|\geq\frac{d^3}8|X_2||X_3|
$$

such [triangles](../../../../../triangle-in-a-graph.md). This proves the asserted bound on exceptional [vertices](../../../../../vertex-graph-theory.md).

There are at least $(1-2\varepsilon)|X_1|\geq|X_1|/2$ good [vertices](../../../../../vertex-graph-theory.md). Summing their [triangle](../../../../../triangle-in-a-graph.md) counts counts each [triangle](../../../../../triangle-in-a-graph.md) with one [vertex](../../../../../vertex-graph-theory.md) in each cluster exactly once, at its $X_1$ [vertex](../../../../../vertex-graph-theory.md). Therefore

$$
\boxed{\#\{\text{triangles in }G\}\geq\frac{d^3}{16}|X_1||X_2||X_3|.}
$$

There is no factor of three to divide out in this cross-cluster count.

This is the [regular triangle counting lemma](../../../../../regular-triangle-counting-lemma.md) with explicit coarse constants.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

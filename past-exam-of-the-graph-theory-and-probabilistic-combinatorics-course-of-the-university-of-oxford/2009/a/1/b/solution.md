<h1 id="a/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the bipartition as $L,R$. Counting edges by their left and right ends gives $2009|L|=2009|R|$, so the parts have equal size. Put $H=G-F$. If some $S\subseteq L$ violated [Hall's marriage theorem](../../../../../hall-s-marriage-theorem.md) in $H$, let $T=N_H(S)$, so $|T|\leq|S|-1$.

There are $2009|S|$ edges of $G$ incident with $S$, of which at most $2009|T|$ can end in $T$. Thus at least $2009(|S|-|T|)\geq2009$ end in $R\setminus T$. All those edges must have been deleted, by the definition of $T$. This contradicts $|F|=2008$. Hence $H$ has a [matching](../../../../../matching-graph-theory-split.md) covering $L$, and equal part sizes make it a **[perfect matching](../../../../../perfect-matching.md) avoiding every edge of $F$**.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

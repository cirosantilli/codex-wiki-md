<h1 id="a/3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Apply part (c) to the pairs $(X_1,X_2)$ and $(X_1,X_3)$. Outside a union of at most $2\epsilon n$ exceptional vertices, every $v\in X_1$ has sets $Y=N(v)\cap X_2$ and $Z=N(v)\cap X_3$ of size at least $dn/2$.

These sets are large enough for epsilon-uniformity of $(X_2,X_3)$, because $d/2>\epsilon$. Hence

$$
e(Y,Z)\geq(d-\epsilon)|Y||Z|\geq\frac d2\left(\frac{dn}2\right)^2=\frac{d^3n^2}8.
$$

Every such edge completes a distinct triangle through $v$. Thus at most $2\epsilon n$ vertices of $X_1$ fail the claimed triangle count. Summing these triangles over the good vertices counts each triangle with one vertex in each class exactly once. Since $d\leq1$ and $\epsilon<d/4\leq1/4$,

$$
\#\{\text{triangles in }G\}\geq(1-2\epsilon)n\frac{d^3n^2}8
\geq\boxed{\frac{d^3n^3}{16}}.
$$

## ↑ Ancestors (13)

1. [D](../d.md)
2. [3](../../3.md)
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

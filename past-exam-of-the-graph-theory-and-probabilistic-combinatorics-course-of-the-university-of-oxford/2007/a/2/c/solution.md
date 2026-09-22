<h1 id="a/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a triangle, $p_{C_3}=x(x-1)(x-2)=(x-1)^3-(x-1)$. For $n\ge4$, deleting an edge leaves a path with polynomial $x(x-1)^{n-1}$, and contracting it leaves $C_{n-1}$. Deletion-contraction and induction give

$$
p_{C_n}=x(x-1)^{n-1}-\{(x-1)^{n-1}+(-1)^{n-1}(x-1)\}
=\boxed{(x-1)^n+(-1)^n(x-1)}.
$$

The path formula chooses its first color freely and each succeeding color in $x-1$ ways.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [A](../../../a.md)
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

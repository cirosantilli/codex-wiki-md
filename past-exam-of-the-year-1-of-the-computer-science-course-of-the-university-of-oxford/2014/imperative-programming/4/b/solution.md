<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [representation invariant](../../../../../representation-invariant.md) is $N\geq0$, `rows.length == N`, and every `rows(i)` is a nonnull finite [list](../../../../../list-abstract-data-type.md) of entries $(j,x)$ satisfying

$$
\boxed{0\leq j<N,\quad x\ne0.0,\quad\text{column indices strictly increase along each row}.}
$$

Strict increase excludes repeated columns. The [abstraction function](../../../../../abstraction-function.md) gives $A_{ij}=x$ when the unique entry $(j,x)$ occurs in `rows(i)`, and $A_{ij}=0$ otherwise. Thus omitted positions represent zero; omission does not mean an unknown [matrix](../../../../../matrix.md) entry.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

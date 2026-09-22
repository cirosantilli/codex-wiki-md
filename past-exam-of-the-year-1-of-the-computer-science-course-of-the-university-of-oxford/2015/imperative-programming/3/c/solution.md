<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [representation invariant](../../../../../representation-invariant.md) is

$$
\boxed{p\ne\mathrm{NIL},\quad p.\mathrm{count}=|\alpha(p.\mathrm{tail})|\geq0,\quad p.\mathrm{tail}\text{ is a finite acyclic chain excluding }p.}
$$

Every reachable non-`NIL` [pointer](../../../../../pointer-computer-programming.md) designates an allocated [linked list node](../../../../../linked-list-node.md) of the appropriate extension type. The header is not a data element. In operations consuming two separate [linked lists](../../../../../linked-list.md), their headers and data chains must additionally be disjoint; this ownership [precondition](../../../../../precondition.md) prevents accidental aliasing during a destructive [merge algorithm](../../../../../merge-algorithm.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

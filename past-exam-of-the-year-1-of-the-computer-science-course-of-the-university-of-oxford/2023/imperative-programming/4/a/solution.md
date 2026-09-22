<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $L(list)$ denote the non-null nodes reachable from the head. The [representation invariant](../../../../../representation-invariant.md) requires a finite acyclic [null-terminated linked list](../../../../../null-terminated-linked-list.md) and pairwise distinct names among its reachable nodes. Names and numbers retain the interface's [string data type](../../../../../string-data-type.md) interpretation; no ordering of names is required.

The [abstraction function](../../../../../abstraction-function.md) is the finite [partial function](../../../../../partial-function.md)

$$
book=\{\,p.name\mapsto p.number\mid p\in L(list)\,\}.
$$

Name uniqueness makes this a [function](../../../../../function-split.md), rather than a relation assigning multiple numbers to one name. Initially `list == null`, so $L(list)=\varnothing$ and **the abstract book is empty**. Unreachable allocated nodes are outside this abstract state.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

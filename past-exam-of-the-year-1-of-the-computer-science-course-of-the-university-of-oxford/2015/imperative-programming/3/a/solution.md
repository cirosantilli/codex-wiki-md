<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For finite acyclic chains, define the [abstraction function](../../../../../abstraction-function.md) recursively by

$$
\boxed{\alpha(\mathrm{NIL})=[],\qquad\alpha(p)=[p]\mathbin{+\!+}\alpha(p.\mathrm{tail})\quad(p\ne\mathrm{NIL}).}
$$

Here the [list](../../../../../list-abstract-data-type.md) contains [linked list nodes](../../../../../linked-list-node.md) themselves. For an extension storing a value `value`, its value-level [abstraction function](../../../../../abstraction-function.md) is $\alpha_v(p)=[p.\mathrm{value}]\mathbin{+\!+}\alpha_v(p.\mathrm{tail})$. Finiteness and absence of a [graph cycle](../../../../../cycle-in-a-graph.md) ensure that these recursive definitions terminate. A [dummy header node](../../../../../sentinel-node.md) is excluded by applying $\alpha$ to its `tail`.

## ↑ Ancestors (12)

1. [A](../a.md)
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

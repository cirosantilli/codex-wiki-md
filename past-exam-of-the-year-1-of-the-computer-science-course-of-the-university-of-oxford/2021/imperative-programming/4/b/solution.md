<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [sentinel node](../../../../../sentinel-node.md) supplies a permanent predecessor for the first real node. Inserting or deleting at the front then uses the same `predecessor.next` update as an interior operation. Its datum is **not a [multiset](../../../../../multiset.md) element**: the chosen extreme [integer](../../../../../integer-split.md) is merely unused sentinel data.

A [representation invariant](../../../../../representation-invariant.md) requires a nonnull fixed header, a finite acyclic chain starting at `bagHeader.next`, and exclusion of the header from that chain. Each node identity occurs once, although different nodes may have equal data. Representation links are owned by the implementation, so outside mutation cannot alter them unexpectedly.

The [abstraction function](../../../../../abstraction-function.md) counts occurrences:

$$
\mathrm{bag}(x)=\bigl|\{u\in L(\mathrm{bagHeader.next}):u.\mathrm{datum}=x\}\bigr|.
$$

This yields nonnegative multiplicities and finite support. Initialization with a null successor gives the empty [multiset](../../../../../multiset.md). Excluding the sentinel is essential even when a real item equals its datum.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

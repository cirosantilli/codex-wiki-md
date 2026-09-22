<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With agent variables, each [constraint domain](../../../../../constraint-domain.md) has [cardinality](../../../../../cardinality.md) $2^m$. Their total number of listed domain values is $n2^m$, while the [Cartesian product](../../../../../cartesian-product.md) of the domains has

$$
\boxed{(2^m)^n=2^{mn}}
$$

complete assignments before constraints.

With item variables, each [constraint domain](../../../../../constraint-domain.md) has [cardinality](../../../../../cardinality.md) $n$. Their total number of listed domain values is $mn$, while their [Cartesian product](../../../../../cartesian-product.md) has

$$
\boxed{n^m}
$$

complete assignments. These are raw domain-space sizes. The larger agent-variable space includes overlaps and missing items; imposing the allocation constraints reduces it to the same $n^m$ actual complete allocations represented directly by item variables.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2023](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)

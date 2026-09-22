<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For finite [lists](../../../../../../list-abstract-data-type.md), [Cartesian lifting of a binary operation to lists](../../../../../../cartesian-lifting-of-a-binary-operation-to-lists.md) preserves [associativity](../../../../../../associative-property.md). Both associations enumerate triples in the same order: the entry from `xs` changes slowest, then the entry from `ys`, then the entry from `zs` changes fastest. The results are respectively

$$
[(x\oplus y)\oplus z\mid x\leftarrow xs;\ y\leftarrow ys;\ z\leftarrow zs]
$$

and

$$
[x\oplus(y\oplus z)\mid x\leftarrow xs;\ y\leftarrow ys;\ z\leftarrow zs].
$$

[Associativity](../../../../../../associative-property.md) makes corresponding entries equal; their order and multiplicity already agree. Empty [lists](../../../../../../list-abstract-data-type.md) make both sides empty. Therefore

$$
\boxed{(xs\,X_\oplus\,ys)\,X_\oplus\,zs=xs\,X_\oplus\,(ys\,X_\oplus\,zs).}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
5. [2003](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)

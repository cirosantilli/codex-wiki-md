<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Read each [Scala trait linearization](../../../../../scala-trait-linearization.md) from the most specific implementation toward the base. For a declaration with parents $P_1,\ldots,P_r$, concatenate their linearizations from right to left, deleting a duplicate from a left operand when it already occurs in the right operand. This can move a repeated ancestor later than a superficial “rightmost trait first” scan suggests. Omitting the common `AnyRef, Any` suffix, the answers are
```
C, Y, H, N, L, I, E
B, Y, H, N, L, D, I, E
A, N, O, Y, S, H, T, L, D, I, E
```
For example, `T` contributes `T,L,D,I,E`, while `O` contributes `O,Y,S,H,E`. In `A`, the separately mentioned `Y` also appears in the later merge with `O`, and `N`'s ancestors also occur in `T`; resolving these duplicates yields the final order displayed above. **The inherited trait orders are the displayed lists after removing their leading class names.** [Class Linearization](../../../../../scala-2-11-classes-and-objects-specification.md)

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

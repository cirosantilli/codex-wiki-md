<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Scala trait linearization](../../../../../scala-trait-linearization.md) merges parent linearizations from right to left, deleting an earlier occurrence when that same ancestor occurs in a later appended parent linearization. Each class precedes its ancestors, and an ancestor appears once.[Class Linearization: concatenation replaces identical elements of its left operand with their occurrences in the right operand; the same rule is used for the Scala 2 code here](../../../../../scala-2-13-classes-and-objects-specification.md) Ignoring the predefined roots gives

| Type | Linearization, most specific first |
| --- | --- |
| `K` | `K` |
| `I` | `I, K` |
| `J` | `J, K` |
| `G` | `G, I, K` |
| `F` | `F, J, I, K` |
| `H` | `H, J, K` |
| `D` | `D, F, J, G, I, K` |
| `E` | `E, H, J, K` |
| `A` | `A, D, F, J, G, I, K` |
| `B` | `B, E, H, D, F, J, G, I, K` |
| `C` | `C, E, H, J, K` |

Each override appends its letter after `super.m` returns. Reading the method chain in reverse from `K` therefore yields the three output lines:

```
KIGJFDA
KIGJFDHEB
KJHEC
```

In particular, mixing `H` into `C` again does not create another `H` or move it before its subclass `E`. Also, `J` lies between `F` and `G` in `D`'s chain; `super` follows the final linearization, not simply one statically named parent.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

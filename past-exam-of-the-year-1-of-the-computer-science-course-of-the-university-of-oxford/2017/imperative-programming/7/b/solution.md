<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Ignoring the predefined universal bases, the [Scala trait linearizations](../../../../../scala-trait-linearization.md) are **`D1, B2, B1, A`** and **`D2, B1, B2, A`**. The rightmost mixed-in trait is searched first, while the shared base occurs only once.

The output is:

```
h in B2, g in B1, f in A
h in B1, g in B2, f in A
```

For `D1`, `h` is the `B2` implementation. Its `super.g` continues after `B2` to `B1.g`; that method's `super.f` continues after `B1` to `A.f`. The second line follows the reversed mixin order. In particular, a trait's unqualified `super` is interpreted in the concrete receiver's linearization, not by assuming the trait always sees only its textual parent.[Class Linearization; Inheritance](../../../../../scala-2-13-classes-and-objects-specification.md)

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

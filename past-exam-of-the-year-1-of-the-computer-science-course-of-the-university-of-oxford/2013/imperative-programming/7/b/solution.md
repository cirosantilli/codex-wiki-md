<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Ignoring predefined ancestors as permitted, the [Scala trait linearizations](../../../../../scala-trait-linearization.md) are

$$
\boxed{D1,B2,B1,A\qquad\text{and}\qquad D2,B1,B2,A.}
$$

A `super` call in a [trait](../../../../../trait.md) continues to the next applicable implementation in the receiver's [Scala trait linearization](../../../../../scala-trait-linearization.md). It is not permanently bound to the parent named when that [trait](../../../../../trait.md) was declared.

For `d1.h`, enter `B2.h`. Its `super.g` reaches `B1.g`, and that method's `super.f` reaches `A.f`. For `d2.h`, enter `B1.h`; its `super.g` reaches `B2.g`, whose `super.f` again reaches `A.f`. Therefore the two output lines are
```
h in B2, g in B1, f in A
h in B1, g in B2, f in A
```
The shared ancestor `A` occurs once in each [Scala trait linearization](../../../../../scala-trait-linearization.md), after the two specialized [traits](../../../../../trait.md). This accounts for the final `f in A` in both lines.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

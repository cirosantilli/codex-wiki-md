<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Each implementation first evaluates `super.meth` and then appends its own name. Consequently the contributions appear in reverse order of the defining traits in the [Scala trait linearization](../../../../../scala-trait-linearization.md). The four printed lines are
```
E I L N H Y 
E I D L N H Y 
E I D L T H S Y O N 
E I D L T H S Y O N 
```
There is a trailing space before each newline. **The third and fourth lines are identical**: the declared type `D` of `o4` permits the call but does not change the actual `A` object's [dynamic dispatch](../../../../../dynamic-dispatch.md) or its `super` chain. Within `N`, for example, `super.meth` in an `A` follows the next implementation in `A`'s full linearization rather than simply using `L` as its isolated textual parent.

## ↑ Ancestors (12)

1. [D](../d.md)
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

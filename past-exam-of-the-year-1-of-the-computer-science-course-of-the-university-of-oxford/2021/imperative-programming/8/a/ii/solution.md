<h1 id="8/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the **[decorator pattern](../../../../../../decorator-pattern.md)**. The wrapper implements the same [object interface](../../../../../../object-interface.md) as its component and delegates before changing the output:

```
class ScaledChannel(inner: Channel, factor: Int) extends Channel {
  override def apply(n: Int): Int = factor * inner(n)
}
```

It can wrap any channel [software object](../../../../../../software-object.md), not only a sum channel. Constructing the wrapper at run time chooses the additional behavior for an existing component, and several wrappers can be composed without adding a subclass for every combination. Each call reaches the wrapped channel once, preserving its state evolution. Scaling the input instead would define a different transformation, particularly for a component that already has history.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [8](../../../8.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)

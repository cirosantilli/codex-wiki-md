<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The standard output is **three lines**:
```
A
2.3
B
```
This is program output, excluding any interactive interpreter's display of returned values. The calls `a.m(1)` and `b.m(5.6)` compute squares without printing. In `A`, the concrete `m(Int)` wins over the [generic method](../../../../../generic-method.md) at argument `1`; the string and `2.3` use `m[T]` and print their arguments.

For `b: B[Any]`, the class [type parameter](../../../../../type-parameter.md) has already become `Any`, so the two alternatives are `m(Any)` and `m(Double)`, rather than a method with its own freely inferred [type parameter](../../../../../type-parameter.md). The `Double` alternative is more specific. It accepts `4` by [numeric widening](../../../../../numeric-widening.md), so `b.m(4)` computes `16.0` without printing; `b.m("B")` prints `B`; `b.m(5.6)` computes a square without printing. These are applications of the [Scala](../../../../../scala.md) 2.11 [method overloading](../../../../../method-overloading.md) rules, with the arithmetic return values discarded in statement position.[Scala 2.11 Language Specification, §6.26.3, overload applicability and specificity](https://www.scala-lang.org/files/archive/spec/2.11/06-expressions.html#overloading-resolution)

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

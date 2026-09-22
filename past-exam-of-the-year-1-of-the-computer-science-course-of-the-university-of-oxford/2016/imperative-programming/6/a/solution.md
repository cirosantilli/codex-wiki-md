<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**The output is `1`, with no newline.** The `Any` in `class B[Any]` and `class C[Any]` is a [type parameter](../../../../../type-parameter.md) name that shadows the standard type `scala.Any` inside those class bodies. Renaming it to `T` preserves the program's meaning. Thus `new B[Int]` has an inherited `m(Double)` and its own `m(Int)`; `obj1.m(1)` selects the latter and prints `1`. The call with `2.3` can only use the inherited `m(Double)`, which computes a sum without printing.

For `new C[Any]`, the supplied [type argument](../../../../../type-argument.md) is the standard `scala.Any`, so the overloads are `m(Double)` and `m(scala.Any)`. The more-specific `Double` alternative accepts `4` by [numeric widening](../../../../../numeric-widening.md), and accepts `5.6` directly. Both return sums without printing. A computed result is not automatically screen output. This reasoning uses the [Scala](../../../../../scala.md) 2.11 overload conventions of Question 5(a); [type erasure](../../../../../type-erasure.md) does not turn either class's generic-argument overload into an [method overriding](../../../../../method-overriding.md) of `m(Double)`.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
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

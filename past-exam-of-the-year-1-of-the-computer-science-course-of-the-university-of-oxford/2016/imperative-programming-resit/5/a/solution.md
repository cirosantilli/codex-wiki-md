<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The output is **`BADDCD`**, without a newline. [Method overloading](../../../../../method-overloading.md) chooses a signature using [static types](../../../../../static-type.md), including the instantiated class [type parameter](../../../../../type-parameter.md); [numeric widening](../../../../../numeric-widening.md) can make a `Double` parameter applicable to an `Int` argument.

- `a.m(o1)` chooses `m(Int)`, which is more specific than the polymorphic method: `B`.
- `a.m(o2)` uses `m[Double](Double)`: `A`.
- `b.m(o1)` compares `m(Any)` and `m(Double)`. `Int` can widen to `Double`, and `Double` is more specific than `Any`: `D`.
- `b.m(o2)` chooses `m(Double)` over `m(Any)`: `D`.
- `c.m(o1)` compares the instantiated `m(Int)` with `m(Double)` and chooses `m(Int)`: `C`.
- `c.m(o2)` can use only `m(Double)`: `D`.

The third call is the subtle one: the existence of `m(Any)` does not prevent the more specific numeric overload from winning. These are Scala 2 [method overloading](../../../../../method-overloading.md) and [numeric widening](../../../../../numeric-widening.md) rules. [Overloading Resolution and Numeric Widening](../../../../../scala-2-11-expressions-specification.md)

## ↑ Ancestors (12)

1. [A](../a.md)
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

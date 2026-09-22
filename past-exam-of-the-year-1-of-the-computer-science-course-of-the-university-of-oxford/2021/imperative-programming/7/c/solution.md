<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Instantiate the two [type parameters](../../../../../type-parameter.md) and implement the [function](../../../../../function-split.md) [object interface](../../../../../object-interface.md):

```
val square: Fun[Int, Int] = new Fun[Int, Int] {
  override def apply(x: Int): Int = x * x
}
```

**[Parametric polymorphism](../../../../../parametric-polymorphism.md)** occurs because the generic [trait](../../../../../trait.md) is specialized by choosing its argument and result types. **[Subtype polymorphism](../../../../../subtype-polymorphism.md)** occurs because the anonymous implementing [software class](../../../../../class-programming.md) is used through a `Fun[Int, Int]` reference; calls to its `apply` operation use the [object interface](../../../../../object-interface.md) contract and [dynamic dispatch](../../../../../dynamic-dispatch.md). [Multiplication](../../../../../multiplication.md) itself is not the second polymorphism needed for this explanation.

For values whose mathematical squares fit in a signed 32-bit [integer](../../../../../integer-split.md), the result is the ordinary square. Outside that range, the supplied [integer](../../../../../integer-split.md) return type cannot represent every mathematical square, and the [multiplication](../../../../../multiplication.md) follows [Scala](../../../../../scala.md) integer-overflow behavior. An implementation requiring exact mathematical results for all [integer](../../../../../integer-split.md) inputs would need a wider result type or an explicit overflow exception.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

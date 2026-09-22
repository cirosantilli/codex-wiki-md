<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An infinite [iterator](../../../../../iterator.md) can keep the current index and triangular value:

```
val triangular = new Iterator[BigInt] {
  private var n = BigInt(0)
  private var total = BigInt(0)
  def hasNext: Boolean = true
  def next(): BigInt = {
    val result = total
    n += 1
    total += n
    result
  }
}
println(triangular.take(8).toList)
```

Before each call, `total` is the [triangular number](../../../../../triangular-number.md) $T_n=n(n+1)/2$. Returning it and then using $T_{n+1}=T_n+n+1$ preserves this invariant. The prefix is **$0,1,3,6,10,15,21,28$**. Arbitrary-precision integers prevent wraparound as the indefinitely available iterator advances.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
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

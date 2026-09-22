<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Keep a running [product](../../../../../../product-of-numbers.md) of the fixed base. In particular, `1.0/n` uses [floating-point arithmetic](../../../../../../floating-point-arithmetic-split.md), avoiding the truncation that [integer division](../../../../../../integer-division.md) would introduce:
```
def eaLinear(n: Int): Double = {
  require(n > 0)
  val base = 1.0 + 1.0 / n.toDouble
  var k = 0
  var result = 1.0
  while (k < n) {
    result *= base
    k += 1
  }
  result
}
```
The [loop invariant](../../../../../../loop-invariant.md) is $0\leq k\leq n$ and $result=base^k$. Initially the empty [product](../../../../../../product-of-numbers.md) is one. Multiplication by `base` and incrementing `k` preserve the [invariant](../../../../../../invariant-mathematics.md). The [loop variant](../../../../../../loop-variant.md) $n-k$ decreases by one. On exit $k=n$, so **the result is $e_a(n)$**, with exactly $n$ multiplications and $O(n)$ [time complexity](../../../../../../time-complexity.md). With `Double`, the operational result is the rounded recurrence, rather than an exact real power; this distinction applies to the next two power computations too.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)

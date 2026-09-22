<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use a `Double` base so that the reciprocal is not truncated by [integer division](../../../../../../integer-division.md). Repeated multiplication gives the requested linear-work approximation to [Euler's number](../../../../../../e-mathematical-constant.md).

```
def eaLinear(n: Int): Double = {
  require(n > 0)
  val base = 1.0 + 1.0 / n.toDouble
  var i = 0
  var result = 1.0
  while (i < n) {
    result *= base
    i += 1
  }
  result
}
```

In exact arithmetic over the [real numbers](../../../../../../real-number.md), the [loop invariant](../../../../../../loop-invariant.md) is $0\leq i\leq n$ and $result=base^i$. It holds initially, one multiplication establishes the next exponent, and at exit $i=n$ gives the specified power. The nonnegative [loop variant](../../../../../../loop-variant.md) is $n-i$. **There are exactly $n$ loop multiplications**, hence $\Theta(n)$ in [asymptotic analysis](../../../../../../asymptotic-analysis.md), and one division to form the base. With [floating-point arithmetic](../../../../../../floating-point-arithmetic-split.md), the invariant describes the intended exact result; the actual output has the corresponding rounding errors.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Imperative programming (resit)](../../../../imperative-programming-resit-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)

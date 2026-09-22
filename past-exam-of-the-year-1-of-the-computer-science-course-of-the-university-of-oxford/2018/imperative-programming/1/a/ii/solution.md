<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use [exponentiation by squaring](../../../../../../exponentiation-by-squaring.md), retaining the unprocessed exponent in `k`:
```
def eaBinary(n: Int): Double = {
  require(n > 0)
  var base = 1.0 + 1.0 / n.toDouble
  var k = n
  var result = 1.0
  while (k > 0) {
    if ((k & 1) != 0) result *= base
    k = k / 2
    if (k > 0) base *= base
  }
  result
}
```
Writing $A=1+1/n$, the [loop invariant](../../../../../../loop-invariant.md) is $k\geq0$ and $result\,base^k=A^n$. If the old exponent is $2q+b$, $b\in\{0,1\}$, multiplying the accumulator by $base^b$ and replacing the remaining power by $(base^2)^q$ preserves the [invariant](../../../../../../invariant-mathematics.md). When $q=0$, the unused squaring may be omitted. The nonnegative [integer](../../../../../../integer-split.md) `k` is a [loop variant](../../../../../../loop-variant.md), since $\lfloor k/2\rfloor<k$ for $k>0$. At exit the remaining power is one, giving **$result=e_a(n)$**. There are $\lfloor\log_2n\rfloor+1$ iterations, at most one accumulator multiplication and one squaring per iteration, hence $O(\log n)$ multiplications and [constant space](../../../../../../constant-space.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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

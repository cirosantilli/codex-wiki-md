<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Maintain an accumulated [array](../../../../../array-data-structure.md) of denominators and an exact remaining [fraction](../../../../../fraction.md). The usual [greedy algorithm](../../../../../greedy-algorithm.md) can require a denominator larger than `Int.MaxValue`, even for an input with `Int` components. The following implementation uses [arbitrary-precision integers](../../../../../arbitrary-precision-integer.md) internally. If that representational limit is reached, it returns the always-valid alternative consisting of `num` copies of $1/den$. Repeated denominators are permitted by the given [Egyptian fraction](../../../../../egyptian-fraction.md) representation.
```
def fromRat(num: Int, den: Int): Array[Int] = {
  require(0 <= num && num < den)
  val start = Reduce(num, den)
  var n = BigInt(start._1)
  var d = BigInt(start._2)
  var e = Array.empty[Int]
  while (n > 0) {
    val q = (d + n - 1) / n
    if (!q.isValidInt) return Array.fill(num)(den)
    e = e :+ q.toInt
    val nextN = n * q - d
    val nextD = d * q
    val g = nextN.gcd(nextD)
    n = nextN / g
    d = nextD / g
  }
  e
}
```
The [loop invariant](../../../../../loop-invariant.md) is $d>0$, $0\leq n<d$, all entries of `e` are positive, and

$$
\sum_{0\leq j<e.length}\frac1{e(j)}+\frac nd=\frac{num}{den}.
$$

Appending $q$ and replacing the residual by $(nq-d)/(dq)$ preserves this equality; division by the [greatest common divisor](../../../../../greatest-common-divisor.md) preserves the residual's value. The [loop variant](../../../../../loop-variant.md) is $n$, by the proof in part (b). If `nextN` is zero, its [greatest common divisor](../../../../../greatest-common-divisor.md) with `nextD` is `nextD`, giving residual $0/1$. On normal exit the residual is zero and **the returned [array](../../../../../array-data-structure.md) has exactly the required value**. On the early-return branch, `num` copies of $1/den$ have that same value directly; the partial [greedy Egyptian fraction expansion](../../../../../greedy-egyptian-fraction-expansion.md) is discarded. `num=0` returns an empty [array](../../../../../array-data-structure.md).

The fallback is a correctness provision for the fixed result type, not an efficiency claim: a large repeated-term [array](../../../../../array-data-structure.md) can be impractical. An [array](../../../../../array-data-structure.md) of [arbitrary-precision integers](../../../../../arbitrary-precision-integer.md) would retain the [greedy Egyptian fraction expansion](../../../../../greedy-egyptian-fraction-expansion.md) without this fallback. Allocation, as with any output-producing program, requires enough available memory. The `BigInt` remainder, [greatest common divisor](../../../../../greatest-common-divisor.md) and checked conversion operations are documented in [Methods gcd, isValidInt and toInt](../../../../../scala-2-12-bigint-api-documentation.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Imperative programming resit](../../../imperative-programming-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

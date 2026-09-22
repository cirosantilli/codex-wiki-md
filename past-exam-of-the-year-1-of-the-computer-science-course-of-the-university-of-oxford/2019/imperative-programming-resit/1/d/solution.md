<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

An [Egyptian fraction](../../../../../egyptian-fraction.md) need not be proper: several positive [unit fractions](../../../../../unit-fraction.md) may sum to at least one. Accordingly, accumulate a general nonnegative [reduced fraction](../../../../../reduced-fraction.md), rather than calling the proper-input-only `Reduce` on every intermediate value. First define an exact helper:
```
def toRatExact(e: Array[Int]): (BigInt, BigInt) = {
  var n = BigInt(0)
  var d = BigInt(1)
  var i = 0
  while (i < e.length) {
    require(e(i) > 0)
    val x = BigInt(e(i))
    val g = d.gcd(x)
    val nextN = n * (x / g) + d / g
    val nextD = d * (x / g)
    val h = nextN.gcd(nextD)
    n = nextN / h
    d = nextD / h
    i += 1
  }
  (n, d)
}

def toRat(e: Array[Int]): (Int, Int) = {
  val result = toRatExact(e)
  require(result._1.isValidInt && result._2.isValidInt,
          "Reduced result does not fit (Int, Int)")
  (result._1.toInt, result._2.toInt)
}
```
The [loop invariant](../../../../../loop-invariant.md) is $0\leq i\leq e.length$, $n\geq0$, $d>0$, $\gcd(n,d)=1$, and

$$
\frac nd=\sum_{0\leq j<i}\frac1{e(j)}.
$$

Writing $g=\gcd(d,x)$, the [fraction](../../../../../fraction.md) for the extended prefix has numerator $n(x/g)+d/g$ and denominator $d(x/g)$. These are the `nextN` and `nextD` in the code. Reducing them preserves the value and restores [coprimality](../../../../../coprime-integers.md). The [loop variant](../../../../../loop-variant.md) is $e.length-i$. At exit **the helper returns the exact sum in lowest terms**, including $(0,1)$ for the empty [array](../../../../../array-data-structure.md).

There are three distinct ways to control [integer overflow](../../../../../integer-overflow.md): cancel the common denominator factor before multiplication, reduce after each addition, and use [arbitrary-precision arithmetic](../../../../../arbitrary-precision-arithmetic.md) when the remaining values still exceed fixed-width bounds. Cancellation reduces intermediate size but cannot guarantee that an exact answer fits `(Int, Int)`. For example, the sum $1/46337+1/46349$ is $92686/2147673613$ in lowest terms, whose denominator exceeds `Int.MaxValue`. No implementation returning that fixed type can represent every permitted input exactly. The wrapper therefore checks this unavoidable result-type limitation instead of silently truncating; `toRatExact` supplies the unrestricted mathematical result.[Checked representability with isValidInt before the potentially truncating toInt conversion](../../../../../scala-2-12-bigint-api-documentation.md)

## ↑ Ancestors (12)

1. [D](../d.md)
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

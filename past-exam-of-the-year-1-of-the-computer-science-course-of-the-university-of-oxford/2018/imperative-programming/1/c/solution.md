<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First rearrange the ratios so that the intermediate powers remain moderate:

$$
e_c(n)=(n+1)\left(1+\frac1n\right)^n-n\left(1+\frac1{n-1}\right)^{n-1}.
$$

This avoids separately forming enormous powers such as $n^n$. Perform the two instances of [exponentiation by squaring](../../../../../exponentiation-by-squaring.md) in one [while loop](../../../../../while-loop.md), using [coupled binary exponentiation](../../../../../coupled-binary-exponentiation.md):
```
def ec(n: Int): Double = {
  require(n > 1)
  val dn = n.toDouble
  var x = 1.0 + 1.0 / dn
  var y = 1.0 + 1.0 / (dn - 1.0)
  var k = n
  var l = n - 1
  var p = 1.0
  var q = 1.0
  while (k > 0 || l > 0) {
    if (k > 0) {
      if ((k & 1) != 0) p *= x
      k /= 2
      if (k > 0) x *= x
    }
    if (l > 0) {
      if ((l & 1) != 0) q *= y
      l /= 2
      if (l > 0) y *= y
    }
  }
  (dn + 1.0) * p - dn * q
}
```
With $A=1+1/n$ and $B=1+1/(n-1)$, the [loop invariant](../../../../../loop-invariant.md) is $k,l\geq0$, $p x^k=A^n$, and $q y^l=B^{n-1}$. Each active branch preserves its own power identity by the parity argument in part (a)(ii), and an inactive branch changes nothing. The [loop variant](../../../../../loop-variant.md) is the mathematical [integer](../../../../../integer-split.md) $k+l$, which need not be computed in a fixed-width variable: it decreases whenever either exponent is positive. At exit $p=A^n$, $q=B^{n-1}$, proving **the returned expression is $e_c(n)$**. There are $O(\log n)$ iterations, at most four loop multiplications each, and two final multiplications. Converting `n` before adding one avoids [integer overflow](../../../../../integer-overflow.md) at `Int.MaxValue`.

The rearrangement avoids [floating-point overflow](../../../../../floating-point-overflow.md) in the original powers, but subtraction still combines two quantities of order $n$ to obtain one of order one. [Catastrophic cancellation](../../../../../catastrophic-cancellation.md) can amplify their accumulated [roundoff error](../../../../../round-off-error.md). The mathematical $O(n^{-2})$ approximation error therefore does not imply that the `Double` implementation improves indefinitely as `n` grows.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

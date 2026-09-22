<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Avoid forming the enormous powers in the original ratios. Put $a=1+1/n$, $b=1+1/(n-1)$ and $k=n-1$; algebra gives

$$
e_c(n)=(n+1)a\,a^k-nb^k.
$$

Use [simultaneous exponentiation by squaring](../../../../../simultaneous-exponentiation-by-squaring.md) to compute the two powers with one loop and a shared remaining exponent:

```
def ec(n: Int): Double = {
  require(n > 1)
  val dn = n.toDouble
  val a = 1.0 + 1.0 / dn
  val b = 1.0 + 1.0 / (dn - 1.0)
  var remaining = n - 1
  var u = a
  var v = b
  var pa = 1.0
  var pb = 1.0
  while (remaining > 0) {
    if (remaining % 2 == 1) {
      pa *= u
      pb *= v
    }
    u *= u
    v *= v
    remaining /= 2
  }
  ((dn + 1.0) * a) * pa - dn * pb
}
```

The exact-arithmetic [loop invariant](../../../../../loop-invariant.md) is $remaining\geq0$, $pa\,u^{remaining}=a^{n-1}$ and $pb\,v^{remaining}=b^{n-1}$. The [even integer](../../../../../even-number.md) and [odd integer](../../../../../odd-integer.md) cases preserve both equalities in parallel. The [loop variant](../../../../../loop-variant.md) is `remaining`. On termination, the displayed expression is exactly the desired approximation in the ideal arithmetic model. For $L=\lfloor\log_2(n-1)\rfloor+1$, the loop uses at most $4L$ multiplications, followed by three more: **$O(\log n)$ multiplications and one loop**.

Converting `n` to `Double` before adding one also avoids overflowing `n + 1` at `Int.MaxValue`. The algebra avoids power overflow but does not remove [catastrophic cancellation](../../../../../catastrophic-cancellation.md): the final subtraction combines quantities of order $n e$ to obtain a result of order $e$. For sufficiently large $n$, [floating-point rounding](../../../../../floating-point-rounding.md) can outweigh the mathematical truncation error. For example, at `n == 1000000` this `Double` computation returns approximately **`2.7180521293`**, although the exact formula is approximately **`2.71828182845916`**. Arbitrarily many requested decimal digits require increased arithmetic precision, not simply a larger `Int` argument.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Place an [implicit conversion](../../../../../implicit-conversion.md) in the companion object and import it into the client scope, so it is available for both an integer argument and an integer receiver:

```
import scala.language.implicitConversions

class Rational(n0: BigInt, d0: BigInt) {
  def this(n: Int, d: Int) = this(BigInt(n), BigInt(d))
  require(d0 != 0)
  private val g = n0.abs.gcd(d0.abs)
  val num: BigInt = (if (d0 < 0) -n0 else n0) / g
  val den: BigInt = d0.abs / g
  def *(r: Rational): Rational =
    new Rational(num*r.num, den*r.den)
  override def toString: String =
    if (den == 1) num.toString else num.toString + "/" + den.toString
}
object Rational {
  implicit def fromInt(n: Int): Rational = new Rational(n,1)
}

import Rational._
val r1 = new Rational(3,7)
val r2 = new Rational(-11,-5)
println(r1*r2)
println(r1*3)
println(7*r1)
```

Normalization gives $r_2=11/5$. The output lines are **`33/35`, `9/7`, `3`**. For `r1*3`, the argument is converted; for `7*r1`, conversion supplies the receiver's rational multiplication method. `BigInt` keeps the exact [rational arithmetic](../../../../../rational-arithmetic.md) independent of fixed-width product overflow.

## ↑ Ancestors (12)

1. [A](../a.md)
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

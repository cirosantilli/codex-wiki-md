<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Maintain opposite signs at the endpoints, rather than assuming that the [polynomial](../../../../../polynomial-split.md) is monotone:

```
def floorRoot(X: Int): Int = {
  require(X > 0 && eval(0.0) <= 0.0 && eval(X.toDouble) > 0.0)
  var lo = 0
  var hi = X
  while (hi - lo > 1) {
    val mid = lo + (hi - lo) / 2
    if (eval(mid.toDouble) <= 0.0) lo = mid
    else hi = mid
  }
  lo
}
```

The [loop invariant](../../../../../loop-invariant.md) is **$0\leq\mathrm{lo}<\mathrm{hi}\leq X$ and $p(\mathrm{lo})\leq0<p(\mathrm{hi})$**. Both branches preserve those signs, even when there are other [roots of a polynomial](../../../../../root-of-a-polynomial.md) or sign reversals elsewhere. When the interval width exceeds one, the midpoint is strictly between its endpoints, so the positive [integer](../../../../../integer-split.md) [loop variant](../../../../../loop-variant.md) `hi - lo` strictly decreases. On exit `hi == lo + 1`, giving the required [postcondition](../../../../../postcondition.md) **$p(\mathrm{lo})\leq0<p(\mathrm{lo}+1)$**. [Continuity](../../../../../continuous-function.md) establishes a [root of a polynomial](../../../../../root-of-a-polynomial.md) between those adjacent [integers](../../../../../integer-split.md), possibly at the left endpoint.

The width is at most halved with rounding upwards, so there are at most $\lceil\log_2X\rceil$ midpoint evaluations, plus two endpoint evaluations in the [precondition](../../../../../precondition.md) check. The midpoint expression avoids adding two large endpoints. The explicit positive upper-bound [precondition](../../../../../precondition.md) supplies the interval order assumed in the question. For the literal computed-`eval` contract, the same proof holds provided evaluated midpoints are not `NaN`; identifying its bracket with the real [polynomial](../../../../../polynomial-split.md) additionally requires trustworthy evaluation signs.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
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

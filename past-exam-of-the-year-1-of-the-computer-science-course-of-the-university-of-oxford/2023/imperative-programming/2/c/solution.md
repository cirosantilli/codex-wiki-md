<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Under exact [integer arithmetic](../../../../../integer-arithmetic.md), the intended result is **$\lceil\log_2 x\rceil$**, using the [ceiling function](../../../../../ceiling-function.md). A sufficient [loop invariant](../../../../../loop-invariant.md) is

$$
i\geq0,\qquad y=2^i,\qquad i=0\ \lor\ 2^{i-1}<x.
$$

Initially $i=0,y=1$, and the final disjunction is true. If the guard holds, the old value $y=2^i$ is below $x$. Incrementing `i` and doubling `y` therefore preserves $y=2^i$ and makes the new lower bound $2^{i-1}<x$ true. At exit $y\geq x$. If $i=0$, positivity of $x$ forces $x=1$; otherwise $2^{i-1}<x\leq2^i$. Both cases establish the claimed [postcondition](../../../../../postcondition.md). Doubling eventually reaches or exceeds any fixed positive $x$, proving [algorithm termination](../../../../../algorithm-termination.md) in this arithmetic model. This is the [doubling-loop ceiling logarithm](../../../../../doubling-loop-ceiling-logarithm.md) argument.

**The printed Scala implementation is not correct for its entire stated `Int` domain.** Its `y` is an `Int`. For $x>2^{30}$, it reaches $y=2^{30}$, wraps to $-2^{31}$ on the next doubling, then becomes zero and stays zero. The guard remains true forever. The [loop invariant](../../../../../loop-invariant.md) above is valid for the printed code only when $1\leq x\leq2^{30}$. Scala documents `Int` as a signed 32-bit value equivalent to Java's primitive `int`.[Scala 2.13.16, class Int: signed 32-bit representation](../../../../../scala-int-api-documentation.md)

A corrected implementation for every positive `Int` input widens the doubling variable before any multiplication:

```
def ceilingLog2(x: Int): Int = {
  require(x > 0)
  var i = 0
  var y = 1L
  while (y < x.toLong) {
    i += 1
    y *= 2L
  }
  i
}
```

Now at most 31 iterations are needed and $y\leq2^{31}$, safely within `Long`. The same [loop invariant](../../../../../loop-invariant.md) proves [total correctness](../../../../../total-correctness.md) without the overflow gap.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

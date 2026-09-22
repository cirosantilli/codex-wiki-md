<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

First find a sign bracket by [exponential search](../../../../../exponential-search.md), then bisect that bracket without evaluating its endpoints again:

```
def floorRoot(): Int = {
  require(eval(0.0) < 0.0)
  var lo = 0
  var hi = 1
  while (eval(hi.toDouble) <= 0.0) {
    lo = hi
    require(hi <= Int.MaxValue / 2, "doubling bound exceeds Int range")
    hi *= 2
  }
  while (hi - lo > 1) {
    val mid = lo + (hi - lo) / 2
    if (eval(mid.toDouble) <= 0.0) lo = mid
    else hi = mid
  }
  lo
}
```

For the first [while loop](../../../../../while-loop.md) the [loop invariant](../../../../../loop-invariant.md) is $p(\mathrm{lo})\leq0$, with `hi` a positive power of two, and either $(\mathrm{lo},\mathrm{hi})=(0,1)$ or $\mathrm{hi}=2\mathrm{lo}$. Every previously tested power of two has nonpositive value. Let $t$ be the least nonnegative [integer](../../../../../integer-split.md) for which $p(2^t)>0$. It exists by the positive [leading coefficient](../../../../../leading-coefficient-of-a-polynomial.md). If the current upper endpoint is $2^k$, a mathematical [loop variant](../../../../../loop-variant.md) is $t-k$ while the guard holds; the next doubling decreases it by one. The first [while loop](../../../../../while-loop.md)'s [postcondition](../../../../../postcondition.md) is $p(\mathrm{lo})\leq0<p(\mathrm{hi})$. The second [while loop](../../../../../while-loop.md) has exactly the invariant, variant and adjacent-integer [postcondition](../../../../../postcondition.md) established in part c.

There are $t+1$ evaluations at powers of two. If $t\geq1$, the final bracket has width $2^{t-1}$ and takes exactly $t-1$ midpoint evaluations. Including the initial sign check, the total is **$2t+1$ evaluations for $t\geq1$, and two for $t=0$**. Thus evaluation cost is $O(\log U)$ for the first positive dyadic bound $U=2^t$; it is not a claim about the first positive [root of a polynomial](../../../../../root-of-a-polynomial.md) when the [polynomial](../../../../../polynomial-split.md) is nonmonotone.

The mathematical argument uses unbounded [integer](../../../../../integer-split.md) endpoints and reliable signs. The guarded `Int` implementation requires the successful dyadic bound to fit in `Int`; otherwise it explicitly fails rather than wrapping to a negative bound. The coefficient assumptions alone cannot guarantee that a requested [integer](../../../../../integer-split.md) result fits a fixed-width type. Floating-point overflow or unreliable signs likewise need a wider or certified evaluator for a fully general implementation.

## ↑ Ancestors (12)

1. [D](../d.md)
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

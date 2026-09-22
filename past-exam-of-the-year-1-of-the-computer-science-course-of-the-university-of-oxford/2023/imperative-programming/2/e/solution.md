<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

To preserve the actual printed function, including its handling of nonpositive exponents and wrapping `Int` bases, use a [tail-recursive](../../../../../tail-recursion.md) accumulator with the same multiplication order:

```
def anotherfuncRec(x: Int, n: Long): Double = {
  require(x > 0)
  @scala.annotation.tailrec
  def loop(y: Int, i: Long, result: Double): Double = {
    if (i <= 0) result
    else {
      val nextResult = if (i % 2 == 1) result * y else result
      loop(y * y, i / 2, nextResult)
    }
  }
  loop(x, n, 1.0)
}
```

Each [recursive call](../../../../../recursive-call.md) corresponds to one source iteration and carries exactly its next [program state](../../../../../program-state.md). Hence it reproduces the printed numerical behavior, rather than silently repairing it. For positive `n`, both routines use $\lfloor\log_2 n\rfloor+1$ steps; for nonpositive `n`, both take constant time. The recursive call is in tail position, so Scala's tail-call optimization avoids a growing [call stack](../../../../../call-stack.md); the annotation asks the [compiler](../../../../../compiler.md) to check that condition.

If the intended exact power is required instead, change the base and accumulator parameters of this same recurrence to `BigInt` and require `n >= 0`, as in part (d). Its mathematical [loop invariant](../../../../../loop-invariant.md) becomes a [recursion invariant](../../../../../recursion-invariant.md), with the same logarithmic number of multiplication steps.

## ↑ Ancestors (12)

1. [E](../e.md)
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

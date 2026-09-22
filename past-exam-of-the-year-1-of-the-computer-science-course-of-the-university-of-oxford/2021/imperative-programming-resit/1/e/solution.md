<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Remove each [prime power](../../../../../prime-power.md) as soon as it is found, and stop trial division once the remaining value has no possible smaller factor:
```
def divisors(n: Int): Int = {
  require(n >= 1)
  var remaining = n
  var factor = 2
  var result = 1
  while (factor.toLong * factor.toLong <= remaining.toLong) {
    var exponent = 0
    while (remaining % factor == 0) {
      remaining /= factor
      exponent += 1
    }
    result *= exponent + 1
    factor += 1
  }
  if (remaining > 1) result *= 2
  result
}
```
At an outer-loop boundary, write $n=q\,remaining$, where $q$ is the product of the [prime powers](../../../../../prime-power.md) already removed. The [invariant](../../../../../invariant-mathematics.md) states that `result` is $\tau(q)$, every prime [divisor](../../../../../divisor.md) of $q$ is smaller than `factor`, and `remaining` has no prime [divisor](../../../../../divisor.md) smaller than `factor`. Thus if `factor` divides `remaining`, it is prime; a composite factor would have a smaller prime [divisor](../../../../../divisor.md), contrary to the [invariant](../../../../../invariant-mathematics.md).

During the inner loop, with $q$ fixed, $n=q\,factor^{exponent}\,remaining$. Each division removes one copy, so the positive remainder strictly decreases and supplies an inner-[loop variant](../../../../../loop-variant.md). On leaving the inner loop the complete power has been removed; multiplying the result by `exponent + 1` uses part (d) and reestablishes the outer [invariant](../../../../../invariant-mathematics.md) after advancing `factor`. The outer factor increases and can never exceed the original $n$ while its guard holds, proving termination.

At exit, a remainder greater than one must be prime: a composite remainder would have a prime factor no larger than its square root, which would still be smaller than `factor`. It therefore contributes one final factor of two. A remainder of one contributes nothing. **The [algorithm](../../../../../algorithm-split.md) returns $\tau(n)$ using constant [auxiliary space](../../../../../auxiliary-space.md) and no [array](../../../../../array-data-structure.md).** The widened multiplication in the loop guard prevents an `Int` overflow in the square test.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
